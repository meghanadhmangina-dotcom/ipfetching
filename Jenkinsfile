pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git ''
            }
        }
        stage('Run Script') {
            steps {
                sh 'chmod +x check_ip.sh'
                sh './check_ip.sh'
            }
        }
    }
}
