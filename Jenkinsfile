pipeline {
  agent any
  stages {
    stage('BuildUtil') {
      steps {
        build(job: 'maven/build.artlab.util', wait: true)
      }
    }

    stage('BuildTelegram') {
      steps {
        build(job: 'maven/build.artlab.telegram', wait: true)
      }
    }

  }
}