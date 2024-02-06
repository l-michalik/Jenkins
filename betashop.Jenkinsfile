pipeline {
    agent none 

    environment {
      GIT_COMMIT= "${COMMIT}"
      SHOP_NAME= "${SHOP_NAME}"
    }

    stages {     
        stage('BETASHOP [ACTION]') {
            steps {
                script {
                    sh "echo SHOP NAME: $SHOP_NAME"
                    sh "echo Environment passed: GIT_COMMIT=$GIT_COMMIT"
                }
            }
        }   
    }
}