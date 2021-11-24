pipeline {
    agent any
    // agent { docker { image 'maven:3.8.4' } }
    stages{
        stage('git'){
            steps {
                sh 'git --version'
            }
        }
        stage('build'){
            steps {
                sh 'mvn --version'
            }
        }
    }
}