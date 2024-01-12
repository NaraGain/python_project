pipeline {
  agent any
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
            sh '''#!/usr/bin/python

python /home/user/dragon.py'''
          }
        }

      }
    }

  }
}