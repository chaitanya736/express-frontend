pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        script {
          // Explicit branch + public repo handling
          git branch: 'main',
              url: 'https://github.com/chaitanya736/express-frontend.git'
        }
      }
    }
    
     stage('Install Dependencies') {
      steps {
        sh 'npm install'
      }
    }

    stage('Restart Flask') {
      steps {
        sh 'pm2 restart express-frontend || pm2 start index.js --name express-frontend'
      }
    }
  }
}
