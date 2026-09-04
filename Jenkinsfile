@Library("shared") _
pipeline{
    agent any
    
    stages{
        stage("Hello"){
            steps{
                Hello()
            }
        }
        stage("Code clone"){
            steps{
                sh "whoami"
                echo "code cloned!"
            }
        }
        stage("Test"){
              steps{
                  echo "Hello Test!"
              }
        }
        
    }
}
