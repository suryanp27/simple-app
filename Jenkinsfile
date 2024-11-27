pipeline { 
  
   agent any

   stages {
   
     stage('checkout') { 
        steps { 
           git branch: 'main', url: 'https://github.com/suryanp27/simple-app.git' 
        }
     }
     
     stage('Test') { 
        steps { 
           sh 'echo "testing application..."'
        }
      }

         stage("Deploy application") { 
         steps { 
           sh 'echo "deploying application...on Dev"'
         }

     }
  
   	}

   }
