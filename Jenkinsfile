pipeline{
  agent any

  stages{
    stage('build') {
      steps {
        echo 'build application with email sending...'
      }
    }
  }

  post {
    always {
     echo 'always !'
    }
    success {
      emailext (to:'cedricmokoko@gmail.com' , body: 'test body', subject: 'test subject jenkins')
    }
  }
}