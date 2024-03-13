pipeline {
    agent any
    environment {
      RELEASE='v1.0'
    }
    stages {
        stage('Build') { 
            agent any
            environment {
              LOG_LEVEL = 'WARNING'
            }
            steps {
              echo "Building the Application ${RELEASE} and the Log level is ${LOG_LEVEL}"  
            }
        }
        stage('Test') { 
            steps {
                echo "Testing the Application ${RELEASE}"  
            }
        }
        stage('Deploy') { 
            steps {
                echo "Deploying the Application ${RELEASE}"  
            }
        }
    }
}
