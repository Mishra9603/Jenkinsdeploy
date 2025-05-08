pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Mishra9603/Jenkinsdeploy.git'
            }
        }

        stage('Deploy (Simulated)') {
            steps {
                bat 'mkdir C:\\deploy\\mysite 2>nul'
                bat 'copy index.html C:\\deploy\\mysite\\index.html'
                echo 'Deployed index.html to C:\\deploy\\mysite'
            }
        }
    }
}
