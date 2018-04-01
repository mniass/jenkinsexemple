pipeline {
    agent any
    options { 
        buildDiscarder(logRotator(numToKeepStr: '1')) 
    }
    parameters {
        string(
            name: 'NAME',
            description: 'Who should I say hello to?',
            defaultValue: 'mniass'
        )    
    }
    stages {
        stage('Build') {
            steps {
                sh 'ansible --version'     
            }
        }
        stage('Test') {
            steps {
                sh "echo ${params.NAME}"
            }    
        }    
    }
}
