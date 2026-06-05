pipeline {
    agent any

    stages {

        stage('Instalar Yarn') {
            steps {
                bat 'npm install -g yarn'
            }
        }

        stage('Instalar Dependências') {
            steps {
                bat 'yarn'
            }
        }

        stage('Instalar Browsers Playwright') {
            steps {
                bat 'yarn playwright install'
            }
        }

        stage('Executar Testes E2E') {
            steps {
                bat 'yarn run e2e'
            }
        }
    }
}