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
                zip zipFile: 'C:\\Users\\maria\\Documents\\5_sem\\Administration\\lab 7\\archive' + env.BUILD_NUMBER.toString() + '.zip', dir: 'C:\\Users\\maria\\Documents\\5_sem\\Administration\\lab 7\\simple_maven'
            }
        }
        stage('Deploy'){
            steps{
                unzip zipFile: 'C:\\Users\\maria\\Documents\\5_sem\\Administration\\lab 7\\archive' + env.BUILD_NUMBER.toString() + '.zip', 
                dir: 'C:\\Users\\maria\\Documents\\5_sem\\Administration\\lab 7\\deploy' + env.BUILD_NUMBER.toString()
            }
        }
    }
}