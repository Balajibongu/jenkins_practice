pipeline {
    agent none
    stages {
        stage('build') {
            steps {
                echo 'this is build phase'
            }
        }
        stage('test') {
            steps {
                echo 'this is test phase'
                echo "Build Number: ${BUILD_NUMBER}"
                echo "Workspace: ${WORKSPACE}"
            }
        }
        stage('deploy') {
            steps {
                echo 'this is deploy phase'
            }
        }
    }
}