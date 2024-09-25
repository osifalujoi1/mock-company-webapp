pipeline{
    /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
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
