node {
stage('SCM Checkout'){
  def mvnHome = tool name: 'Maven', type: 'maven'

git 'https://github.com/Bibhuranjan/Devops_test'
}
stage('compile-package'){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh"${mvnHome}/bin/mvn package"
}
}
