pipeline {
    agent {
        label 'sandbox'
    }
    
    stages {
        stage('Build') {
            steps {
                echo "Build Apps"
                sleep(5)
            }
        }
        stage('Test'){
            parallel {
                stage('Test A') {
                    steps {
                         echo "Test A"
                         sleep(5)
                    }
                }
                stage('Test B') {
                    steps {
                         echo "Test B"
                         sleep(5)
                    }
                }
                stage('Test C') {
                    steps {
                         echo "Test C"
                         sleep(5)
                    }
                }
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploy Apps"
            }
        }
    }
}