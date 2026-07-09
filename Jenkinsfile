pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting source code'
            }
        }

        stage('Run Script') {
            steps {
                sh './hello.sh'
            }
        }

        stage('Finish') {
            steps {
                echo 'Pipeline finished'
            }
        }
    }
}