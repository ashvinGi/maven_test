@Library("mylibrary")_

pipeline
{
    agent any
    stages
    {
        stage("Continouse-Download_Master")
        {
            steps
            {
                script
                {
                    
                 cicd.newGit("https://github.com/ashvinGi/maven.git")
                        
          }
                
            }
            
        }
        
        stage("Continouse-Build_Master")
        {
            steps
            {
                script
                {
                    
                 cicd.newMaven()
                    
                    
                }
                
            }
            
        }
        
        stage("Continouse-Deploy_Master")
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
        stage("Continouse-Test_Master")
        {
            steps
            {
                script
                {
                    
                 cicd.newTest("${JOB_NAME}")
                    
                    
                }
                
            }
            
        }
         stage("Continouse-Delivery_Master")
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
