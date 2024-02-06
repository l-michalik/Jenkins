Pipeline {
    agent none 

    environment {
      MY_ENV = "Devops"
      GIT_COMMIT= "${COMMIT}"
    }

    stages {     
        stage('Demoshop') {
            steps {
                script {
                    sh "echo Demoshop"
                    sh "echo Hello $MY_ENV"
                    sh "echo Environment passed: GIT_COMMIT=$GIT_COMMIT"
                }
            }
        } 
    }
}