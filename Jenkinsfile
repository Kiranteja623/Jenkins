pipeline {
  agent { node { label 'ubuntu' } }
  stages {
    stage('git clone') {
      steps {
                git 'https://github.com/Kiranteja623/openmrs-core.git'
                branch 'declarative'
            }
    }
    stage('build') {
    steps {
        sh 'mvn clean package'
    }
  }
  }
}