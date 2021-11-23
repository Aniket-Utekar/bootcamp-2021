pipeline {
  agent any
  stages {
    stage("cleaning stage") {
      steps {
        echo "test"
      }
    }
    stage("Testing stage") {
      steps {
        echo "testing stage"
      }
    }
    stage("packaging stage") {
      steps {
        echo "packaging stage"
      }
    }
    stage("send email") {
      steps {
        mail bcc: '', body: 'Jenkins Job status', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'aniket.annie017@gmail.com'
      }
    }
  }
}
