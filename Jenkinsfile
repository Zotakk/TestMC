pipeline {
  agent none
  stages {
    stage('step 1 ') {
      steps {
        mail(subject: 'Test mail', body: 'Hola! ', from: 'rrcansino@gfi.es', to: 'fphilip@houseware.es', cc: 'sbeltran@gfi.es')
        sleep 60
        error 'ERROR!'
      }
    }
  }
}