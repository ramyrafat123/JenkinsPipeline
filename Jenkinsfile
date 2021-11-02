pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Building the .NET Core App'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing The App'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying The app in IIS'
      }
    }

  }
}