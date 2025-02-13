pipeline {
  agent { label 'docker-agent' } // Use your Docker agent label
  stages {
    stage('Checkout') {
      steps {
        git(
          url: 'git@github.com:your-username/django-app.git',
          credentialsId: 'github-creds', // Match your credential ID
          branch: 'main'
        )
      }
    }
  }
}
