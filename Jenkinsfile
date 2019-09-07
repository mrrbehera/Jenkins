pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'HelloPipeline1'
          }
        }
        stage('Stage2') {
          steps {
            echo 'this is hello from stage2'
          }
        }
      }
    }
    stage('BlueStage1') {
      steps {
        sleep 1
      }
    }
  }
}