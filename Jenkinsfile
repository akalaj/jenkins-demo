pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'This is build number $BUILD_NUMBER for the pipeline $DEMO'
        sh ' echo "This is build $BUILD_NUMBER for $DEMO"'
      }
    }

  }
  environment {
    DEMO = 'DEMO1'
  }
}