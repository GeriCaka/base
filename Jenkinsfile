pipeline {
  agent any
  
  parameters {    
    string(name: 'Workspace', defaultValue: 'NONE', description: 'Workspace')
    booleanParam(name: 'Build', defaultValue: true, description: 'Run Build')
    booleanParam(name: 'StageA', defaultValue: true, description: 'Run stage A')
    booleanParam(name: 'StageB', defaultValue: true, description: 'Run stage B')
    booleanParam(name: 'StageC', defaultValue: true, description: 'Run stage C')
  }
  
  stages {  
    
    stage ('prova') {
      steps {
        echo "${currentBuild.getBuildCauses()}"
      }
    }
    
    stage('Build') {
       when {
        expression { return params.Build }
      }
      steps {
        bat """
        cd ${params.Workspace}
        dir
        mvn clean install
        """       
      }
    }
    
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
