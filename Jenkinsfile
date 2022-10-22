pipeline {
  agent any
  stages {
    stage('Gitintigeration') {
      steps {
        echo 'git connection'
      }
    }

    stage('BUILD') {
      parallel {
        stage('BUILD') {
          steps {
            echo 'Build step'
          }
        }

        stage('Code quality validation') {
          steps {
            echo 'code quality verification'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }

  }
}