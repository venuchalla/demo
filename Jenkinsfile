pipeline {
    agent any
tools {
        maven 'Maven 3.8.1'
        jdk 'jdk8'
    }
    stages {
    stage ('Initialize') {
                steps {
                echo 'intializing...'
                    sh '''
                        echo "PATH = ${PATH}"
                        echo "M2_HOME = ${M2_HOME}"
                    '''
                }
            }
    }
    stage ('bulid') {
                    steps {
                      echo 'cleaning step...'
                      sh 'mvn clean'
                      echo 'installing step...'
                      sh 'mvn install'
                    }
                }
        }
}