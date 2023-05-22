@Library("mylibrary")_

pipeline
{
    agent any
    stages
    {
        stage("Continouse-Download")
        {
            steps
            {
                script
                {
                    
                 cicd.newGit("https://github.com/ashvinGi/maven.git")
                        
          }
                
            }
            
        }
        
        stage("Continouse-Build")
        {
            steps
            {
                script
                {
                    
                 cicd.newMaven()
                    
                    
                }
                
            }
            
        }
        
        stage("Continouse-Deploy")
        {
            steps
            {
                script
                {
                    
                 cicd.newDeploy("${JOB_NAME}","172.31.47.227","testapp")
                    
                    
                }
                
            }
            
        }
        
         stage("Continouse-Selinium-Download")
        {
            steps
            {
                script
                {
                    
                 cicd.newGit("https://github.com/ashvinGi/FunctionalTesting.git")
                    
                    
                }
                
            }
            
        }
        stage("Continouse-Test")
        {
            steps
            {
                script
                {
                    
                 cicd.newTest("${JOB_NAME}")
                    
                    
                }
                
            }
            
        }
         stage("Continouse-Delivery")
        {
            steps
            {
                script
                {
                    
                 cicd.newDeploy("${JOB_NAME}","172.31.47.227","prodapp")
                    
                    
                }
                
            }
            
        }     
    }
      
}
