pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
               git branch: 'main', credentialsId: 'b7ca5726-9935-4f3c-acd7-6de755612133', url: 'https://github.com/manik-93/exp4j.git'
            }
        }
stage('Compile') {
            steps {
              javac App.java
            }
        }

stage('Run') {
            steps {
               bat java App
            }
        }
    }
}
