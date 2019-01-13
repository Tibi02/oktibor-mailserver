node('master') {
   ws('/disk/docker/poste.io') {
      stage('Git checkout') {
         ansiColor('xterm') {
            checkout scm
         }
      }
   
      stage('Compose pull') {
         ansiColor('xterm') {
            sh 'docker-compose pull'
         }
      }
   
      stage('Compose up') {
         ansiColor('xterm') {
            sh 'docker-compose up -d'
         }
      }
   }
}