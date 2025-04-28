pipeline {
    agent any
    stages {
        stage('Construir imagen') {
            steps {
                sh 'docker-compose build'
            }
        }
        stage('Levantar servicios') {
            steps {
                sh 'docker-compose up -d'
            }
        }
    }
}

