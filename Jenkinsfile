pipeline {
    agent any
    environment {
      DISABLE_AUTH = 'true'
      DB_ENGINE    = 'sqlite'
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    printenv
                '''
            }
        }
    }
}
