pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile.build'
    }

  }
  stages {
    stage('step 1 ') {
      steps {
        mail(subject: 'Test mail', body: 'Hola! ', from: 'rrcansino@gfi.es', to: 'fphilip@houseware.es', cc: 'sbeltran@gfi.es')
        sleep 60
        error 'ERROR!'
      }
    }
  }
  environment {
    dir = 'build'
    label = 'my-defined-label'
    additionalBuildArgs = '--build-arg version=1.0.2'
  }
}