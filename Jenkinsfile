node{
    stage('Clone') {
        checkout scm
    }
    stage('Ansible') {
      ansibl-playbook (
          colorized: true, 
          become: true,             
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
