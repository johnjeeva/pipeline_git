

pipeline {
    agent { any { image 'maven:3.8.4-openjdk-11-slim' } }
    stages {
        stage('build') {
            steps {
                   script {
                    if (ENVIRONMENT_NAME == 'development') {
                        ENV_NAME = 'Development'
                    } else if (ENVIRONMENT_NAME == 'release') {
                        ENV_NAME = 'Production'
                    }
                }
            }
        }
    }
}

