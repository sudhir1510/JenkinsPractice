pipeline {
         agent any
 
         withCredentials([
      [$class: 'UsernamePasswordMultiBinding', credentialsId: curl_pass, usernameVariable: 'Username', passwordVariable: 'Password'],
    ]){
    
    stages {
        stage ('echo variables') {
          sh """(
            echo "User: ${Username}"
            echo "Pass: ${Password}"
          )"""
        }                                                                                                                                                  
         }
    }
}
