pipeline {
    agent { 
        node {
            label 'linux'
            }
      }
    
    
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                
                sh '''
                python3 --version
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                python3 py1.py
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
