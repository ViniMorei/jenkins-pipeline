pipeline {
    agent any  // Usa qualquer agente Jenkins disponível

    stages {
        stage('Checkout') {
            steps {
                echo 'Clonando o repositório...'
                checkout scm  // Clona o repositório configurado no Jenkins
            }
        }

        stage('Build') {
            steps {
                echo 'Construindo o projeto...'
                sh 'echo "Build iniciado"'
            }
        }

        stage('Test') {
            steps {
                echo 'Rodando testes...'
                sh 'python3 src/main.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Fazendo o deploy...'
                sh 'echo "Deploy concluído"'
            }
        }
    }
}
