pipeline{
    agent any
    tools {
        nodejs 'NodeJS 14'
    }
    stages{
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
