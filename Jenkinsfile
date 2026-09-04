@Library('Shared')_
pipeline{
    agent any
    
    stages{
        stage("Code clone"){
            steps{
                sh "whoami"
            clone("https://github.com/rohitgargfzr/django-notes-app.git","main")
            }
        }
        stage("Test"){
              steps{
                  echo "Hello Test!"
              }
        }
        stage("Code Build"){
            steps{
            dockerbuild("notes-app","latest")
            }
        }
        stage("Push to DockerHub"){
            steps{
                dockerpush("dockerHubCreds","notes-app","latest")
            }
        }
        stage("Deploy"){
            steps{
                deploy()
            }
        }
        
    }
}
