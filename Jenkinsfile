pipeline {
  agent any
  stages {
    stage('checkout') {
      parallel {
        stage('checkout') {
          steps {
            git(url: 'https://github.com/NaraGain/python_project.git', branch: 'main', changelog: true)
          }
        }

        stage('excute python file') {
          steps {
            sh '''#check file ls file
ls -l

cat dragon.py

python dragon.py
'''
          }
        }

        stage('checkdevbranch') {
          steps {
            git(url: 'https://github.com/NaraGain/python_project.git', branch: 'dev')
          }
        }

      }
    }

    stage('checkoutversion') {
      steps {
        sh 'git --version'
      }
    }

  }
}