pipeline {
    agent {
        docker { image 'node:24-alpine' }
    }
    stages {
        stage('Clone the repos') {
            steps {
                echo 'Cloning backend repository'
                git branch: 'main',
                    url: 'https://github.com/w-burgis/devops-er-backend.git'
                echo 'Was backend cloned?'
                sh 'ls -a'
            }
        }
    }
}
