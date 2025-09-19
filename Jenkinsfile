pipeline {
    agent {
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning the Git repository...'
                git branch: 'main', url: 'https://github.com/SaiKrishnaG19/FilmCastPro-Infra.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing Node.js dependencies...'
                sh 'npm install'
            }
        }

        stage('Build App') {
            steps {
                echo 'Building the React application...'
                sh 'npm run build'
            }
        }
    }
}
