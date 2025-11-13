pipeline {
  agent any

  stages {
    stage('Checkout Source') {
      steps {
        echo "🔄 Checking out main branch..."
        git branch: 'main', url: 'https://github.com/Nareshgundavelli/kubernetes-.git'
      }
    }
  }

  post {
    success { echo "✅ Checkout completed." }
    failure { echo "❌ Checkout failed." }
  }
}
