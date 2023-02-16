pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o work work.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        sh 'work --test'
        echo 'Test Stage Successful'
        
    }
}
    stage('Deploy'){
      steps{
//         sh './work'
        echo 'Deploy Stage Successful'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
