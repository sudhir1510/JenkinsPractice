pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'cd d:'
                echo "on d drive"
                bat 'D:\\new.bat'
                
            }
        }
        stage('mask password') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'curl_pass', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                      sh 'curl -u $USERNAME:$PASSWORD http://localhost:8080'
                    }
                
            }
        }
        
        
    }
}
