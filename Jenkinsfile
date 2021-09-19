pipeline {
    agent any 
    environment {
        // Using returnStdout
        CC = """${sh(
                returnStdout: true,
                script: 'aws s3 ls'
            )}""" 
        // Using returnStatus
        EXIT_STATUS = """${sh(
                returnStatus: true,
                script: 'exit 1'
            )}"""
    }
    stages {
        stage('Example') {
            environment {
                DEBUG_FLAGS = '-g'
            }
            steps {
                sh 'echo "$CC"'
                sh 'echo "$EXIT_STATUS"'
            }
        }
    }
}
