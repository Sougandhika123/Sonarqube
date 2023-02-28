pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
         stage('Test') {
            steps {
                echo 'Test App'
            }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Summery', subject: 'Build status', to: 'sougandhika1998@gmail.com'
        }
    }
}
