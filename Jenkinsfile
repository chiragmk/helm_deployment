pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'make' 
                archiveArtifacts artifacts: '**/mysql_project/*helmignore', fingerprint: true 
            }
        }
    }
}
