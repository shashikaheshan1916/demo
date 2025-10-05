pipeline {
  agent any
  triggers { pollSCM('H/5 * * * *') }

  stages {
    stage('Checkout') {
      steps {
        echo "Checked out ${env.BRANCH_NAME} from ${env.GIT_URL ?: 'SCM'}"
      }
    }
    stage('Build') {
      steps { echo 'Build stage (placeholder)' }
    }
    stage('Unit & Integration Tests') {
      steps { echo 'Run tests (placeholder)' }
    }
    stage('Code Analysis') {
      steps { echo 'Static analysis (placeholder)' }
    }
    stage('Security Scan') {
      steps { echo 'Security scan (placeholder)' }
    }
    stage('Deploy to Staging') {
      steps { echo 'Deploy to staging (placeholder)' }
    }
    stage('Integration Tests on Staging') {
      steps { echo 'Integration tests on staging (placeholder)' }
    }
    stage('Deploy to Production') {
      steps { echo 'Deploy to prod (placeholder)' }
    }
  }

  post {
    always {
      echo "Build finished with status: ${currentBuild.currentResult}"
    }
  }
}


