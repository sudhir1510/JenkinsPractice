pipeline {
         agent any
   
         node{
         
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
}
