
pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/gopal2804/Jenkins-git-integration.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x HelloWorld.java"
                javac "HelloWorld.java"
                java "HelloWorld"
            }
        }
     stage('Test Code') {
            steps {
                echo "testing stage done"
            }
        }
    } 
}
