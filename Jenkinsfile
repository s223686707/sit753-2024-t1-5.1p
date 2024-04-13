pipeline {
    environment {
        DIRECTORY_PATH = '/Users/subhash/Downloads/Masters In Information Technology (Professional)/Trimester 1 2024/SIT753 Professional Practice in IT/TASK 5.1P/sit753-2024-t1-5.1p'
        TESTING_ENVIRONMENT = 'testing'
        PRODUCTION_ENVIRONMENT = 'Subhash'
    }

    agent any

    stages {
        stage('Build') {
            steps {
                echo "Fetch the source code from the directory path specified by the environment variable: ${env.DIRECTORY_PATH}"
                echo "Compile the code and generate any necessary artifacts"
            }
        }

        stage('Test') {
            steps {
                echo "Unit tests"
                echo "Integration tests"
            }
        }

        stage('Code Quality Check') {
            steps {
                echo "Check the quality of the code"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy the application to a testing environment specified by the environment variable: ${env.TESTING_ENVIRONMENT}"
            }
        }

        stage('Approval') {
            steps {
                sleep 10
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploy the application to the production environment: ${env.PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}