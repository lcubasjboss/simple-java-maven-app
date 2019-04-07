pipeline {
    agent any
    stages {
        stage('Build') {
            steps {            
                checkout scm
                echo "OK Checkout"
            }
        }
        
        stage('Test') {
            steps {
                sh '/maven/apache-maven-3.6.0/bin/mvn -version'
                echo "OK Mvn version"
            }
            /*
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }*/
        }
        /*
        stage('Deliver') {
            steps {
                sh './jenkins/scripts/deliver.sh'
           }
        }*/
    }
}
