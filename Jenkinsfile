pipeline {
  agent any
  stages {
    stage('Stage 0 : start') {
      steps {
        echo 'Hi, starting now'
        emailext(subject: 'p2210-django - pipeline runining', attachLog: true, to: 'simohamed.seddik@outlook.fr', body: 'new pipeline runining')
        mail(subject: 'p2210-django', body: 'p2210-django', to: 'simohamed.seddik@outlook.fr')
      }
    }

    stage('Stage 1 : Build') {
      steps {
        echo '== TEST =='
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