pipeline {
    agent any
    stages{
        stage('git'){
            steps {
                bat 'git --version'
            }
        }
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