pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                archiveArtifacts artifacts: '**/mysql_project/*helmignore', fingerprint: true 
            }
        }
    }
}
