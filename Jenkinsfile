pipeline {
    agent any
    stages {
       
        stage('mask password') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'curl_pass', usernameVariable: 'Username', passwordVariable: 'Password')]) {
                      sh 'curl -u $USERNAME:$PASSWORD http://localhost:8080'
                    }
                
            }
        }
        
        
    }
}
