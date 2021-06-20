pipeline {
    agent any

    stages {
    stage('clean') {
                steps {
                    echo 'cleaning workspace..'
                    mvn clean
                    echo 'cleaning workspace completed'
                }
            }
        stage('validate') {
            steps {
                echo 'validating.....'
                 mvn validate
                  echo 'validating is completed.....'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                mvn test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                mvn install
            }
        }
    }
}