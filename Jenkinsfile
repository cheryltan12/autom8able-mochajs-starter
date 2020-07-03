pipeline {
    agent any

    stages {
        stage('start') {
            steps{
                echo 'Starting..'
                notifyStarted()
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'npm run test:awesome'
            }
        }

    }
