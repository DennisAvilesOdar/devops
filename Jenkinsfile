pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        slackSend(color: 'good', message: 'Iniciando deploy')
        ansiblePlaybook(playbook: '/Users/dennisavilesodar/Developer/practica/devops/produccion.yml', colorized: true, inventory: '/Users/dennisavilesodar/Developer/practica/devops/host')
      }
    }

  }
}