pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/willwugit/hello-devops.git'
            }
        }


        stage('Run Script') {
            steps {
                sh '''
                chmod +x hello.sh
                ./hello.sh
                '''
            }
        }


        stage('Finish') {
            steps {
                echo 'Pipeline finished'
            }
        }

    }
}