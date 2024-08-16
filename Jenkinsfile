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
    success {
      //Utilisation des valeurs customs
      //emailext (to:'cedricbayito@gmail.com' , body: 'test body', subject: 'test subject jenkins')
      
      //Utilisation des valeurs par defaut de jenkins
      emailext (to:'cedricbayito@gmail.com' , body: '$DEFAULT_CONTENT', subject: '$DEFAULT_SUBJECT')
    }
  }
}