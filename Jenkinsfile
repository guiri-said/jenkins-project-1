pipeline {
    agent any
    stages {
        stage('Pull') {
            steps {
                sh "rm -rf *"
                git branch: 'main', url: 'https://github.com/guiri-said/jenkins-project-1.git'
            }
        }
        stage('Build') {
            steps {
                sh "javac Main.java"
            }
        }
        stage('Run') {
            steps {
                sh "java Main"
            }
        }
    }
}
