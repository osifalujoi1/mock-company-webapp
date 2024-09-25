pipeline{
    agent any

    stages{
        stage('Install Yarn') {
            steps {
                sh 'npm install -g yarn'
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
