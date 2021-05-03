node{
  stage('Checkout SCM'){
    git 'https://github.com/sirikdevops/my-app'
  }
  stage('clean-compile-package'){
   def mvnPath = tool name: 'maven3.6.3', type: 'maven'
    sh "${mvnPath}/bin/mvn package"
  }
}
