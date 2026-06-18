
pipeline {
    agent any

    stages {

        stage('Python Version') {
            steps {
                bat '"C:\\Users\\pk599\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\pk599\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Users\\pk599\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m py_compile app.py'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploy Successful'
            }
        }
    }
}