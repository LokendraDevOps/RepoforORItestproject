pipeline {
    agent { lable 'Slave-1' }
    environment {
        APP_NAME = "SimpleWebApp"
        DEPLOY_DIR = "/var/www/html"
        }
        stages {
            stage('Checkout') {
                steps {
                    git branch: 'main', url: 'https://github.com/LokendraDevOps/RepoforORItestproject.git'
                }
            }
            stage('copy files') {
                steps {
                sh 'sudo cp -rf . /var/www/html/'
                }
            }
        }
    }
