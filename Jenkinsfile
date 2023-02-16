pipeline { 
  agent any
  stages { 
    stage('Build') { 
       steps { 
        echo 'Build Stage Successful'
       } 
    }
    stage('Test') { 
       steps { 
        echo 'Test Stage Successful' 
       }
    }
//         post { 
//           always { 
//             junit 'target/surefire-reports/*.xml
//           }
//         }
//  }
//    } 
    stage('Deploy') { 
//       steps { 
          echo 'Deployment Successful'
      }
    }
}
post {
      failure {
        echo 'Pipeline failed'
      }
    }
}
