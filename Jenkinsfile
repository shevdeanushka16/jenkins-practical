
pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking GitHub repository'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build successful-polling test'
            }
        }

        stage('Test') {
            steps {
                echo 'Second Test successful '
            }
        }
    }
}
