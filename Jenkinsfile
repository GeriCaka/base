pipeline {
  agent any
  
  parameters {
    choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
    booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
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
