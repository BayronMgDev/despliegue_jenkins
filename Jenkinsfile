pipeline {
    agent any
    stages {

        stage('Build') {
            steps {
                echo "Etapa de build no disponible"
            }
        }
        stage('Test') {
            steps {
                echo "Etapa de Test no disponible"
            }
        }
        stage('Deploy') {
            steps {
                sh "docker-compose down -v"
                sh "docker-compose up -d --build"
            }
        }
    }
    post {
        always {
            cleanWs()
        }
    }
}
