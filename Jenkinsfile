pipeline {
    agent any
    
    stages{('Build'){
        steps{
            bat 'python app.py'
        }
    }
    stage ('Test'){
        steps {
            bat 'exit 1'
        }
    }
    }
}