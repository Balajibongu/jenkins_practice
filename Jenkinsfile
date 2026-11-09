pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'this is build phase'
            }
        }
        stage('test') {
            steps {
                echo 'this is test phase'
                sh 'whoami'
                sh 'pwd'
                sh 'ls -la'
            }
        }
        stage('deploy') {
            steps {
                echo 'this is deploy phase'
            }
        }
    }
    post {
        always {
            echo "In here we will clean all the jenkin files in workspace directory"
            cleanWs()
        }
    }
}