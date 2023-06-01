pipeline
{
  agent any
  stages{
    stage('A'){
      steps{
        git credentialsId: '4aad631f-78a1-441b-9dd7-5ecc0501bb1c', url: 'https://github.com/HKMtech123/github_youtube.git'
      }
    }
}
  
  post{
    success{
      sh 'tar -cvf file.tar /var/lib/jenkins/workspace/github_pipeline/'
    }
    failure{
      sh 'date'
    }
    always{
      sh 'ifconfig enp0s3'
    }
  }

}


