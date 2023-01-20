pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing is happening...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying is happening.....'
            }
          
        }
        
    }
    post{
        always{
        emailext body: 'Summary', replyTo: 'thisiswasimnc@gmail.com', subject: 'Jenkins Pipeline', to: 'thisiswasimnc@gmail.com'
        }
    }
}
