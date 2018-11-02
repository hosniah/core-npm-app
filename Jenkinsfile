pipeline {
  agent {
    kubernetes {
      label 'mypodtemplate-npm-6'
      defaultContainer 'node-container'
      yaml 'KubernetesPod.yaml'
    }
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}
