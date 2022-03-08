pipeline {
    agent any

    stages {
        stage('Python') {
            steps {
                bat 'posnegint.py'
            }
        }
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
