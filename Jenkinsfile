pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/pavithra-m13/sample_1.git'
            }
        }

        stage('Build') {
            steps {
                echo 'No build needed for static HTML'
            }
        }

        stage('Deploy to Apache') {
            steps {
                echo 'Deploying HTML files to Apache server'
                // Clean the old files
                // sh 'sudo rm -rf /var/www/html/*'
                // Copy new files
                // sh 'sudo cp -r * /var/www/html/'
            }
        }
    }

    post {
        success {
            echo 'Deployment successful!'
        }
        failure {
            echo 'Deployment failed!'
        }
    }
}
