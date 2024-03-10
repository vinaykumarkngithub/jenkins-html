pipeline {
  agent any
  stages {
    stage('Fetch the Code') {
      steps {
        git(url: 'https://github.com/vinaykumarkngithub/jenkins-html.git', branch: 'main')
      }
    }

    stage('Install Apache2') {
      steps {
        sh 'sh \'sudo apt install apache2 -y\''
      }
    }

    stage('Deploy the App') {
      steps {
        sh 'sh \'sudo cp -R * /var/www/html\''
      }
    }

  }
}