pipeline {
    agent any
    stages {
        stage('Create Deployment') {
            steps {
                sh 'kubectl apply -f Deployment.yml'
            }
        }
        stage('Expose Deployment using LoadBalancer') {
            steps {
                sh 'kubectl apply -f Service.yml'
            }
        }
    }
}