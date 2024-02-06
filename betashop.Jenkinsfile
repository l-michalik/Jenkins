Pipeline {
    agent none 

    environment {
      MY_ENV = "Devops"
      GIT_COMMIT= "${COMMIT}"
    }

    stages {     
        stage('Betashop') {
            steps {
                script {
                    sh "echo Betashop"
                    sh "echo Hello $MY_ENV"
                    sh "echo Environment passed: GIT_COMMIT=$GIT_COMMIT"
                }
            }
        } 
    }
}