pipeline {
  agent any
  stages {
    stage('Stage 0 : start') {
      steps {
        echo '== Stage 0 : Start =='
      }
    }

    stage('Stage 1 : Build') {
      steps {
        echo '== Stage 1 : Start =='
        git 'https://github.com/mohsadki/p2210-django.git'
      }
    }

    stage('Stage 2 : Lunch') {
      steps {
        pwd()
        git(url: 'https://github.com/mohsadki/p2210-django.git', branch: 'main', poll: true)
      }
    }

  }
}