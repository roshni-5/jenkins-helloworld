pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        
        stage('Test') {
            when {
                expression { return false }  // Change to false to skip test
            }
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
    
    post {
        always {
            echo 'Pipeline completed'
        }
    }
}
