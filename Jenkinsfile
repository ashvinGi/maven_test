@Library("mylibrary")_

pipeline
{
    agent any
    stages
    {
        stage("Continouse-Download_Lone")
        {
            steps
            {
                script
                {
                    
                 cicd.newGit("https://github.com/ashvinGi/maven.git")
                        
          }
                
            }
            
        }
        
        stage("Continouse-Build_Lone")
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
      







