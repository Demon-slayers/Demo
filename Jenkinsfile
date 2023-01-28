pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Buildinggg...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing is happening....'
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
        emailext body: 'Summary', replyTo: 'shonitaric@gmail.com', subject: 'Jenkins Pipeline', to: 'shonitaric@gmail.com'
        }
    }
}
