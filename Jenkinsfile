pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git 'https://github.com/pandian3k/Maven-Demo.git' 
      }
    }
    stage('build') {
      steps {
        bat 'mvn install'
      }
    }
    stage('deploy') {
      steps {
        sh 'cp -r "C:\\\\Program Files (x86)\\\\Jenkins\\\\workspace\\\\maven pipeline1\\\\mave\\\\multi-module\\\\webapp\\\\target\\\\webapp.war" "C:\\\\Program Files\\\\Apache Software Foundation\\\\Tomcat 8.5\\\\webapps"'
      }
    }
  }
 }
