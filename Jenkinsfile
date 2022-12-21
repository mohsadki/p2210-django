pipeline {
  agent any
  stages {
    stage('Stage 0 : start') {
      steps {
        echo 'Hi, starting now'
        emailext(subject: 'p2210-django - pipeline runining', attachLog: true, to: 'simohamed.seddik@outlook.fr', body: 'new pipeline runining')
      }
    }

    stage('Stage 1 : build') {
      steps {
        timestamps() {
          sh 'echo "test"'
        }

      }
    }

    stage('Stage 2 : Test') {
      steps {
        echo '== TEST =='
      }
    }

  }
}