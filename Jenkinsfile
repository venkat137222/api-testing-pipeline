pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install -g newman'
            }
        }

        stage('Run Postman Tests') {
            steps {
                sh '''
                newman run collection/sample_api_collection.json
                '''
            }
        }
    }
}
