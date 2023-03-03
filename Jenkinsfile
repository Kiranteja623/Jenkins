pipeline {
  agent any
  stages {
    stage('git clone') {
      steps {
                git 'https://github.com/Kiranteja623/openmrs-core.git'
                branch 'declarative'
            }
    }
    stage('build the  package') {
      steps {
          sh 'cd /openmrs-core'
          sh 'mvn clean package'
      }
    }
  }}