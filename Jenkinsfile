pipeline {

   agent any
   tools {
    nodejs '15.2.0'
   }

   options {
    timeout(time:2,unit:'MINUTES')
   }

   stages {
    stage('Instalando dependencias') {
      sh 'npm install'
    }

    stage('Corriendo test') {
      sh 'npm test'
    }

    stage('Final') {
      echo 'Fin del pipeline'
    }

   }

}
