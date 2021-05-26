pipeline {
  agent {
    node {
      label 'test'
    }

  }
  stages {
    stage('mkdir') {
      steps {
        fileExists 'E:\\\\jenkins-test'
        sh 'mkdir -p E:\\\\jenkins-test\\\\test1\\\\test1'
      }
    }

    stage('rmdir') {
      steps {
        sh 'rm -rf E:\\\\jenkins-test\\\\test1\\\\test1'
      }
    }

  }
  environment {
    node1 = 'master'
  }
}