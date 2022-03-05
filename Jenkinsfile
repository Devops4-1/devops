pipeline{
  agent any
  stages{
    stage("git checkout")
    {
      steps
    {
      git branch: 'develop', credentialsId: 'github-cred', url: 'https://github.com/Devops4-1/devops.git'
    }
    }
    
    stage("devops")
    {
      steps {
            echo "devops"
          }
     }
  }
   }
