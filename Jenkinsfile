pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'make check'
            }
        }
    }
    post {
        always {
            junit '**/target/*.xml'
        }
        failure {
           emailext body: 'Your Build is successful', subject: 'Build is successfull', to: 'thisiswasimnc@gmail.com'
        }
    }
}
