node{
  stage('SCM Checkout'){
    git 'https://github.com/mandeeps-cloud/my-app-master'
  }
  stage('Compile-Package){
  sh 'mvn package'
  }
}
