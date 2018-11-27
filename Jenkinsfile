node {
stage('SCM Checkout'){
  def JAVA_HOME = tool name: 'Java', type: 'jdk'

git 'https://github.com/Bibhuranjan/Devops_test'
}
stage('compile-package'){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh"${mvnHome}/bin/mvn package"
}
}
