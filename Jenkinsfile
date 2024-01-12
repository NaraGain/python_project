pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/NaraGain/python_project.git', branch: 'main')
      }
    }

    stage('check file') {
      steps {
        sh '''ls -lrt
'''
      }
    }

  }
}