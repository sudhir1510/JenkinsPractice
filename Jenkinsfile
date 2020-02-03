pipeline {
         withCredentials([
      [$class: 'UsernamePasswordMultiBinding', credentialsId: curl_pass, usernameVariable: 'Username', passwordVariable: 'Password'],
    ]){
    agent any
   
    stages {
        stage('Build') {
            steps {
                bat 'cd d:'
                echo "on d drive"
                bat 'D:\\new.bat'
                
            }
        }       
        stage ('echo variables') {
          sh """(
            echo "User: ${Username}"
            echo "Pass: ${Password}"
          )"""
        }
    }                                                                                                                                                  
    }
    }
}
