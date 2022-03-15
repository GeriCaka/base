pipeline {
  agent any
  
  parameters {    
    booleanParam(name: 'StageA', defaultValue: true, description: 'Run stage A')
    booleanParam(name: 'StageB', defaultValue: true, description: 'Run stage B')
    booleanParam(name: 'StageC', defaultValue: true, description: 'Run stage C')
  }
  
  stages {
    stage('stageA') {
      when {
        expression { return params.StageA }
      }
      steps {
        echo 'Inside stageA'
      }
    }
    
    stage('stageB') {
      when {
        expression { return params.StageB }
      }
      steps {
        echo 'Inside stageB'
      }
    }
    
    stage('stageC') {
      when {
        expression { return params.StageC }
      }
      steps {
        echo 'Inside stageC'
      }
    }
    
  }
}
