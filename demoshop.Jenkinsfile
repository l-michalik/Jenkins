pipeline {
    agent none 

    environment {
      GIT_COMMIT= "${COMMIT}"
    }

    stages {     
        stage('DEMOSHOP [ACTION]') {
            steps {
                script {
                    sh "echo Environment passed: GIT_COMMIT=$GIT_COMMIT"
                }
            }
        }   
    }
}