node {    
    scmVars = checkout scm

    sh 'mkdir -p devops'
	  dir("devops")
    {
        script{
            git branch: "main", 
                url: 'https://github.com/l-michalik/Jenkins.git'            
        }
    }

    script {
      if(true){
        withEnv(["COMMIT=${scmVars.GIT_COMMIT}","BRANCH=${scmVars.GIT_BRANCH}"]) {    
          load 'demoshop.Jenkinsfile'  
        }
      }else{
        withEnv(["COMMIT=${scmVars.GIT_COMMIT}","BRANCH=${scmVars.GIT_BRANCH}"]) {    
          load 'betashop.Jenkinsfile'  
        }
      }
    }
} 