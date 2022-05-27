pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        slackSend(color: 'good', message: '"${env.JOB_NAME} - ${env.BUILD_DISPLAY_NAME} - Iniciando deploy"')
        ansiblePlaybook(playbook: '/Users/dennisavilesodar/Developer/practica/jenkins/data/jobs/devops/branches/master/workspace/produccion.yml', colorized: true, inventory: '/Users/dennisavilesodar/Developer/practica/jenkins/data/jobs/devops/branches/master/workspace/host')
      }
    }

  }
}