pipeline {
    agent any
    stages{
        stage('clone'){
            steps {
                bat 'clone.bat'
            }
        }
        stage('build'){
            steps {
                bat 'build.bat'
            }
        }
        stage('test'){
            steps {
                bat 'test.bat'
            }
        }
    }
}