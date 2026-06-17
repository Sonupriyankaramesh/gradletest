pipeline {
    agent any

    tools {
        gradle 'Gradle'
    }

    stages {

        stage('Check') {
            steps {
                sh 'which gradle'
                sh 'gradle --version'
                sh 'java -version'
            }
        }

        stage('Checkout') {
            steps {
                git 'https://github.com/Sonupriyankaramesh/gradletest.git'
            }
        }

        stage('Build') {
            steps {
                sh 'gradle build'
            }
        }

        stage('Run') {
            steps {
                sh 'gradle run'
            }
        }
    }
}
