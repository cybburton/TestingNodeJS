pipeline {
  agent {
    docker {
      image '/Users/cyb.burton/Downloads/master-vert.yaml'
      args 'stage'
    }

  }
  stages {
    stage('') {
      steps {
        node(label: 'start') {
          ws(dir: '/Users/cyb.burton/Downloads') {
            build 'master-vert'
          }

        }

      }
    }
  }
  environment {
    stage = '1'
  }
}