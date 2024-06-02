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
                    dir('maven-project') {
                        sh 'mvn clean install'
                    }
                }
            }
        }
        
        stage('Build with Gradle') {
            steps {
                script {
                    echo 'Building project with Gradle...'
                    dir('gradle-project') {
                        sh 'gradle build'
                    }
                }
            }
        }

        stage('Build with Node.js') {
            steps {
                script {
                    echo 'Building project with Node.js...'
                    dir('nodejs-project') {
                        sh 'npm install'
                        sh 'npm run build'
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
