pipeline {
         agent any
 
    stages {
             
         withCredentials([
      [$class: 'UsernamePasswordMultiBinding', credentialsId: curl_pass, usernameVariable: 'Username', passwordVariable: 'Password'],
    ]){
    
        stage ('echo variables') {
          sh """(
            echo "User: ${Username}"
            echo "Pass: ${Password}"
          )"""
        }                                                                                                                                                  
         }
    }
}
