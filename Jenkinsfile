pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        npm install
        npm run build
      }
    }
  }
}
