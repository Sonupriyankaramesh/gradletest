pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Sonupriyankaramesh/gradletest.git'
            }
        }
        stage('Build') {
            steps {
                sh './gradlew clean build'
            }
        }

        stage('Run') {
            steps {
                sh './gradlew run'
            }
        }
    }
}
