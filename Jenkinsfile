pipeline {
  agent any
  environment {
    chromeDriverPath = '/Users/jorge.quiros/qa/jenkinsPipeline'
  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'starting our pipeline'
          }
        }

        stage('Test') {
          steps {
            echo 'testing our app'
            echo "Chromedriver path is ${chromeDriverPath}"
          }
        }

      }
    }

    stage('Deployment') {
      steps {
        echo 'Deploying to AWS'
      }
    }

  }
}