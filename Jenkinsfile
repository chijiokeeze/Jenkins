pipeline {
    agent any
    stages {
        stage('download stage') {
            steps {
                sh 'echo download has been executed'
            }
        }
        stage('Build stage') {
            steps {
                sh 'echo Build stage has is been executed'
            }
        }
        stage('init test stage') {
            agent {
                docker {
                    image 'maven'
                }
            }
            steps {
                sh 'mvm --version'
                sh 'echo MAVEN was executed'
            }
        }
       
    }           
}
