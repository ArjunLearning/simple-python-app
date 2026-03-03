pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'python app.py'
            }
        }

        stage('Test') {
            steps {
                bat '''
                echo Running validation...
                if not exist app.py (
                    echo ERROR: app.py missing
                    exit 1
                )
                echo Validation passed
                exit 0
                '''
            }
        }
    }
}