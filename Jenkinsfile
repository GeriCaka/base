pipeline {
  agent any
  
  parameters {    
    booleanParam(name: 'StageA', defaultValue: true, description: 'Run stage A')
    booleanParam(name: 'StageB', defaultValue: true, description: 'Run stage A')
    booleanParam(name: 'StageC', defaultValue: true, description: 'Run stage A')
  }
  
  stages {
    stage('stageA') {
      steps {
        echo 'Inside stageA'
      }
    }
    
    stage('stageB') {
      steps {
        echo 'Inside stageB'
      }
    }
    
    stage('stageC') {
      steps {
        echo 'Inside stageC'
      }
    }
    
  }
}
