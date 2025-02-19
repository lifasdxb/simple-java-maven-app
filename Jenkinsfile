pipeline {
    agent any
    tools {
        maven 'Maven' // Matches the Maven name in Global Tool Configuration
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
                sh 'echo "PATH: $PATH"' // Debug PATH inside Jenkins
                sh 'which mvn' // Check if Maven is accessible
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
