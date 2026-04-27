pipeline {
    agent any

    tools {
        maven 'Maven3'
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/rihabchk/TPJavaPipeLine-NakraMohallirRihab.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

    }
}
