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
            echo 'Get The Diver Path ${ChromeDriverPath}}'
          }
        }

        stage('TestLog') {
          steps {
            echo 'Message Log'
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
  environment {
    ChromeDriverPath = 'C:\\Driver\\test.exe'
  }
}