node {
stage('SCM Checkout'){
  def JAVA_HOME = tool name: 'java', type: 'jdk'
  -Djdk.net.URLClassPath.disableClassPathURLCheck=true

git 'https://github.com/Bibhuranjan/Devops_test'
}
stage('compile-package'){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh"${mvnHome}/bin/mvn package"
}
}
