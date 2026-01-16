pipeline {
    agent any

    stages {
        stage('Fetch Local IP') {
            steps {
                script {
                    def localIP = sh(
                        script: "hostname -I | awk '{print $1}'",
                        returnStdout: true
                    ).trim()
                    echo "Local IP Address: ${localIP}"
                }
            }
        }
    }
}
