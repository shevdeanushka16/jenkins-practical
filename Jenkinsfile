
pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking GitHub repository'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage'; bat 'echo build completed'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Test successful'
            }
        }
    }
post{
    success{echo 'pipeline completed successfully'}
    failure{echo 'pipeline failed'}
}
}
