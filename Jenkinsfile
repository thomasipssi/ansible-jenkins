node{
    stage('Clone') {
        git 'https://github.com/thomasipssi/ansible-jenkins.git'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,            
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
