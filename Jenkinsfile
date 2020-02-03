pipeline {
         agent any
 
    stages {
    
        stage ('echo variables') {
                 
                          
         withCredentials([
      [$class: 'UsernamePasswordMultiBinding', credentialsId: 'curl_pass', usernameVariable: 'Username', passwordVariable: 'Password'],
    ]){
    
          sh """(
            echo "User: ${Username}"
            echo "Pass: ${Password}"
          )"""
        }                                                                                                                                                  
         }
    }
}
