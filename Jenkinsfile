pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', credentialsId: '46cd66c2-3836-4d2b-b366-f00124452f25', url: 'https://github.com/Anudharane/TEIT21.git'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac hello.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java hello'
            }
        }
    }
}



