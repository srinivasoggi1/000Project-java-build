pipeline {
    agent any
    tools {
        maven 'myMaven'
    }
    stages {
        stage ('get code') {
            steps {
                git 'https://github.com/efsavage/hello-world-war.git'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}