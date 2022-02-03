node{
    stage('Clone') {
        git 'https://github.com/ludovic-tech/ansible-jenkins.git'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,            
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
