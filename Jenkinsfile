pipeline {
    agent any

    tools {
        maven 'M3'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -B package'
            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn -B deploy'
            }
        }
    }
}
