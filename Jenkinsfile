pipeline{
    agent any 
    stages {
        stage('Git Checkout'){  
            steps{   
                git branch: 'main', url: 'https://github.com/Chakravarthy18/demo-counter-app.git'
            }
        }
        stage('unit testing'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Integration testing'){
            steps{
                sh 'mvn verify -DskiUnitTests'
            }
        }
    }
}
    