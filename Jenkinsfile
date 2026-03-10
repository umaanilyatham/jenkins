pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/umaanilyatham/jenkins.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                bat 'wsl ansible-playbook -i inventory deploy.yml'
            }
        }

    }
}
