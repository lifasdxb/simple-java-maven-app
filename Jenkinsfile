
pipeline {
    agent any
    tools {
        maven 'Maven' // This should match the name you set in Global Tool Configuration
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}