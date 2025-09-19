pipeline {
    agent {
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning the Git repository...'
                git branch: 'main', url: 'git@github.com:SaiKrishnaG19/FilmCastPro.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing Node.js dependencies...'
                sh 'npm install'
            }
        }

        stage('Build React App') {
            steps {
                echo 'Building the React application...'
                sh 'npm run build'
            }
        }
    }
}
