pipeline{
    agent any

    tools{
        jdk 'java-11'
        maven 'maven'
    }

    stages{
        stage('git checkout'){
            steps{
                git branch: 'main',url:'https://github.com/sakshi-kp/project-1.git'
            }
        }
        stage('Build'){
            steps{
                sh "mvn clean install"
            }
        }
        stage('compile'){
            steps{
                sh "mvn compile"
            }
        }
    }
}