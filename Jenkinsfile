pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               script{
					dir(mysql_project){
					sh("helm install . --generate-name")
					}
					
			   }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
