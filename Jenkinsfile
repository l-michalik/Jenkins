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
    
    // pass the environment variables to new pipeline
    withEnv(["COMMIT=${scmVars.GIT_COMMIT}","BRANCH=${scmVars.GIT_BRANCH}"]) {    
        // load Jenkinsfile Pipeline file from devops repository     
        load 'demoshop.Jenkinsfile'  
    }
} 