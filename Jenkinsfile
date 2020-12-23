pipeline {

   agent any
   tools {
    nodejs 'Node 15.2.0'
   }

   options {
    timeout(time:2,unit:'MINUTES')
   }

   stages {
    stage('Instalando dependencias') {
      steps {
        sh 'npm install'
      }
    }

    stage('Corriendo test') {
      steps{
        sh 'npm test'
      }

    }

    stage('Final') {
      steps{
        sh 'echo "Termina el pipeline y la version de node es: "$(node --version)'
      }

    }

   }

}
