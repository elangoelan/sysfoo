pipeline {
    agent any
    stages {
        stage('Step 1 ------- Packaging') {
            steps {
              sh "mvn packages"
            }
        }
		stage('Step 2 archive artifacts') {
            steps {
             archiveArtifacts artifacts: '**/*.war', fingerprint: true
            }
        }
}
}
