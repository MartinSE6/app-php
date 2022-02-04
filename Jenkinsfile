node{
    stage('Clone') {
        checkout scm
    }
    stage('Ansible') {
      ansible-playbook (
          colorized: true, 
          become: true,             
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
