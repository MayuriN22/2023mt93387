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
        
        
    }
}
