node{
    stage('Clone') {
        git 'https://github.com/Jesuipssi/ansible-jenkins.git'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,            
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
