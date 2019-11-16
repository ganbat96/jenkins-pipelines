pipeline {
  agent any
  stages {
    stage('BuildUtil') {
      steps {
        build(job: 'maven/build.artlab.util', wait: true)
        sh 'echo \'ganbbat\''
        echo 'hey'
      }
    }

    stage('BuildTelegram') {
      steps {
        build(job: 'maven/build.artlab.telegram', wait: true)
      }
    }

  }
}