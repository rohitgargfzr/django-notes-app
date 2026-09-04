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
        
    }
}
