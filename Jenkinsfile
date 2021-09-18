pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                retry(3) {
                    sh 'echo fail; exit 1'
                }

                timeout(time: 3, unit: 'MINUTES') {
                    sh 'echo done'
                }
            }
        }
    }
}
