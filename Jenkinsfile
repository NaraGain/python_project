pipeline {
  agent {docker {images 'python:3.5.1'} }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/NaraGain/python_project.git', branch: 'main')
      }
    }

    stage('check file') {
      parallel {
        stage('check file') {
          steps {
            sh '''ls -lrt
'''
          }
        }

        stage('run python file') {
          steps {
            sh 'ls -a && sh "python ./dragon.py"'
          }
        }

      }
    }

  }
}
