pipeline {
    agent any
    environment{
        PROJECT = 'roboshop'
        LANGUAGE= 'groovy'
    }
    stages {
        stage('build') {
            steps {
                echo 'this is build phase'
                echo "this project name is: ${PROJECT}"
                echo "this project language: ${LANGUAGE}"
            }
        }
        stage('test') {
            steps {
                echo 'this is test phase'
                // sh 'whoami'
                // sh 'pwd'
                // sh 'ls -la'
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