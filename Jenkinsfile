pipeline {
    agent any
tools {
        maven 'Maven 3.8.1'
        jdk 'jdk8'
    }
    stages {
             stage ('Initialize') {
                           steps {
                              
                           }
            }

           stage ('bulid') {
                       steps {

                      mvn clean
                      mvn install
                    }
                }
    }
}