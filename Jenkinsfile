pipeline {
  agent none
  stages {
    stage('step 1 ') {
      parallel {
        stage('step 1 ') {
          steps {
            mail(subject: 'Test mail', body: 'Test numero 3!', from: 'jenkinsOceanBlue@gfi.es', to: 'rrcansino@gfi.es')
            sleep 15
          }
        }
        stage('') {
          steps {
            echo 'Mail enviado'
          }
        }
      }
    }
  }
}