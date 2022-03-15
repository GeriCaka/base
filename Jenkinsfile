pipeline {
  agent any
  
  parameters {    
    booleanParam(name: 'StageA', defaultValue: true, description: 'Run stage A')
    booleanParam(name: 'StageB', defaultValue: true, description: 'Run stage B')
    booleanParam(name: 'StageC', defaultValue: true, description: 'Run stage C')
  }
  
  stages {
    stage('stageA') {
      steps {
        echo 'Inside stageA'
        echo "${StageA}"
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
