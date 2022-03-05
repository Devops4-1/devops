pipeline{
  agent any
  stages{
    stage("git checkout")
    {
      steps
    {
      checkout([$class: 'GitSCM', branches: [[name: '*/develop']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-cred', url: 'https://github.com/Devops4-1/devops.git']]])
    }
    }
    
    stage("devops")
    {
      steps {
            cleanWs cleanWhenAborted: false, cleanWhenFailure: false, cleanWhenNotBuilt: false, cleanWhenUnstable: false
          }
     }
  }
   }
