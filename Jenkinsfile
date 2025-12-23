pipeline {
    agent any
    tools {
        // Attention: Assurez-vous que Maven est configuré sous le nom "Maven" dans Jenkins
        // (Manage Jenkins > Global Tool Configuration)
        maven 'Maven' 
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'mvn test'
            }
        }
    }
}
