pipeline {
    agent any
    tools {
       maven 'maven3'
    }
    stages{
        stage('Build'){
            steps{
                 sh script: 'mvn clean package'
                 sh script: echo "Hello World"
            }
        }
    }
}
