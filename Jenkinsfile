pipeline {
  agent { label 'docker-agent' } // Use your Docker agent label
  stages {
    stage('Checkout') {
      steps {
        git(
          url: 'https://github.com/gauravkr0007/E-Commerce-projects.git',
          //credentialsId: 'github-creds', // Match your credential ID
          branch: 'main'
        )
      }
    }
  }
  post {
        always {
            echo 'Job finished!'
        }
        success {
            echo 'Job succeeded!'
        }
        failure {
            echo 'Job failed!'
        }
    }
}
