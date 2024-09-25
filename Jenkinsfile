pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git url: 'https://github.com/osifalujoi1/mock-company-webapp', branch: 'main'
            }
        }
        stage('Build'){
            steps{
                sh './gradlew assemble'
            }
        }
        stage('Test'){
            steps{
                sh './gradlew test'
            }
        }
    }
}
