node{
  stage('SCM Checkout'){
    
    git 'https://github.com/mandeeps-cloud/my-app-master'
  }
  stage('Compile-Package'){
  //Get Maven Home Path
  def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email Notifications'){    
      mail bcc: '', body: '''Hi Welcome to Email Alerts
      Thanks
      Mandeep''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'monteoberoigcp9@gmail.com'
  }
}
