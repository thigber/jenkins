pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Validar HTML') {
            steps {
                echo 'Verificando se o arquivo index.html existe...'
                sh 'test -f index.html' // Verifica se o arquivo está lá
                echo 'HTML validado com sucesso!'
            }
        }
        stage('Deploy Simulado') {
            steps {
                echo 'Copiando index.html para o servidor de produção...'
                // Aqui simularíamos o envio para um servidor Apache/Nginx
                echo "O site de Thiago Bergamaschi foi atualizado!"
            }
        }
    }
}