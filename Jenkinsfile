pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from your repository
                git 'https://github.com/MayuriN22/2023mt93387.git'
            }
        }
        
        stage('Build and Compile') {
            steps {
                // Build your project (e.g., with Maven, Gradle, etc.)
                sh 'mvn clean install'
            }
        }
        stage('Run Application') {
            steps {
                script {
                    if (isUnix()) {
                        // Unix-specific commands
                        sh 'nohup java -jar BuildMayuri_Assignment.jar &'
                    } else {
                        // Windows-specific commands
                        bat 'start java -jar BuildMayuri_Assignment.jar'
                    }
                }
            }
        }
        
        
    }
}
