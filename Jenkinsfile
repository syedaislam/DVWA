pipeline {
  agent any
  stages {
    stage('stage01') {
      steps {
        dependencyCheck(odcInstallation: 'owasp', additionalArguments: '--format HTML --format XML')
        dependencyCheckPublisher()
      }
    }

  }
}