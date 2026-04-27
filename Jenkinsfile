pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/rihabchk/TPJavaPipeline-NakraMohallirRihab.git'
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
