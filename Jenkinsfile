pipeline{
    agent any
    tools{
        nodejs 'Node JS'
    }
    stages{

        stage('Check Node') {
            steps{
                sh 'node --version'
                sh 'npm --version'
            }
        }
        stage('Run') {
            steps{
                sh 'npm start'
            }
        }
    }
    post{
        always{
            cleanWs()
        }
    }
}