node {
stage('SCM Checkout'){
  def JAVA_HOME = tool name: 'java', type: 'jdk'
  JENKINS_JAVA_OPTIONS="-Djdk.net.URLClassPath.disableClassPathURLCheck=true"

git 'https://github.com/Bibhuranjan/Devops_test'
}
stage('compile-package'){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh"${mvnHome}/bin/mvn package"
}
  stage('Sonarqube-Analysis') {
      def mvnHome = tool name: 'Maven', type: 'maven'
    withSonarQubeEnv('sonarqube') {
      sh "${mvnHome/bin/mvn sonar:sonar" 
    }
  }
}
