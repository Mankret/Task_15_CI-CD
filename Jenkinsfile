pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                sh 'curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -'
                sh 'apt install -y nodejs'
            }
        }
        stage('Build') {
            steps {
                sh 'npm -v'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Jenkins URL: $JENKINS_URL"'
            }
        }
    }
}

