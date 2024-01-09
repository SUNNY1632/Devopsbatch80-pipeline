pipeline {
  agent any
  stages {
    stage('Commit') {
      steps {
        echo 'commit the code'
      }
    }

    stage('BUILD') {
      steps {
        echo 'BUILD THE CODE'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test the code'
          }
        }

        stage('Stage') {
          steps {
            echo 'stage the code'
          }
        }

        stage('Deploy') {
          steps {
            echo 'deploy the code'
          }
        }

        stage('Operate') {
          steps {
            echo 'operate the code'
          }
        }

      }
    }

  }
}