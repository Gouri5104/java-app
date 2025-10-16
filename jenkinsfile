pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Gouri5104/java-app.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'    // use 'sh' if on Linux
            }
        }

        stage('Run Application') {
            steps {
                bat 'mvn exec:java'        // execute the main class
            }
        }
    }
}
