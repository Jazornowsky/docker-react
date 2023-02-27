pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile.dev'
            dir 'build'
            label 'jazornowsky/docker-react'
            args: '-e CI=true'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}