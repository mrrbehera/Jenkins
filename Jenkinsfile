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
            build(job: 'hp1', quietPeriod: 2)
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