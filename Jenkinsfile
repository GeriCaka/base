pipeline {
  agent any
  
  parameters {
    choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
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
