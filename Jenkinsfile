node{
    stage('Clone') {
        checkout scm
    }
    PATH = "/usr/bin/ansible:/usr/bin/ansible-playbook:$PATH"
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true, 
          become: true,             
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
