pipeline {
  agent any
  stages {
    stage("run frontend") {
      steps {
        echo 'executing yarn...'
        nodejs('NodeJS') {
          sh 'yarn install'
        }
      }
    }
    stage("run backend") {
      steps {
        echo 'exectuing gradle...'
        Gradle() {
          sh './gradlew -v'
        }
      }
    }
  }
}
