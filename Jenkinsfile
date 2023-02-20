pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG20CS348.cpp -o PES1UG20CS348'
                 build job: 'PES1UG20CS348-1', wait: false
                 echo 'Build successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG20CS348.cpp'
                echo 'Test successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
