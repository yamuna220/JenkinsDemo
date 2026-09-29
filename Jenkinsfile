pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                sh 'javac src/Main.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java -cp src Main'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}