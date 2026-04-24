pipeline {
    agent any
    
    environment {
        PROJECT_VERSION = '1.1.0'
        PROJECT_NAME = 'HelloWorld'
    }
    
    stages {
        stage('Build') {
            steps {
                echo "Building ${PROJECT_NAME} version ${PROJECT_VERSION}"
                echo "Build ID: ${env.BUILD_ID}"
                echo "Job Name: ${env.JOB_NAME}"
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        
        stage('Deploy') {
            steps {
                echo "Deploying version ${PROJECT_VERSION}"
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed'
        }
    }
}
