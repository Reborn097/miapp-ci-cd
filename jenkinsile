pipeline {
    agent any
    stages {
        stage('Clonar') {
            steps {
                git 'https://github.com/Reborn097/miapp-ci-cd.git'
            }
        }
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
