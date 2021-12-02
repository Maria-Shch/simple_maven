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
        stage('archive'){
            steps {
                bat 'clone.bat'
            }
        }
        stage('Deploy'){
            steps{
                bat 'clone.bat'
            }
        }
    }
}