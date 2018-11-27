node {
stage('SCM Checkout'){
  tool name: 'Maven', type: 'maven'

git 'https://github.com/Bibhuranjan/Devops_test'
}
stage('compile-package'){
sh'mvn package'
}
}
