node{
  stage('SCM Checkout'){
    
    git 'https://github.com/mandeeps-cloud/my-app-master'
  }
  stage('Compile-Package'){
  //Get Maven Home Path
  def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
