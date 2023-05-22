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
        
        
            
        }
    }
      







