pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/yparent/ajc.git"
            }
        }
        stage('build') {
            steps {
                sh "cd ajc/ && javac Main.java"
            }
        }
        stage('run') {
            steps {
                sh "cd ajc/ && java Main"
            }
        }
    }
}
