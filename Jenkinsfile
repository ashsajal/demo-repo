pipeline {
    agent any

    tools {
        maven 'maven' // Define Maven tool
        gradle 'gradle' // Define Gradle tool
        nodejs 'nodejs' // Define Node.js tool
    }

    stages {
        stage('Build with Maven') {
            steps {
                script {
                    echo 'Building project with Maven...'
                    
                    }
                }
            }
        }
        
        stage('Build with Gradle') {
            steps {
                script {
                    echo 'Building project with Gradle...'
                    
                    }
                }
            }
        }

        stage('Build with Node.js') {
            steps {
                script {
                    echo 'Building project with Node.js...'
                    
                    }
                }
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully!'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
