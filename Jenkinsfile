pipeline { 
  
   agent any

   stages {
   
     stage('checkout') { 
        steps { 
           git branch: 'main', url: 'https://github.com/suryanp27/simple-app.git' 
        }
     }
     
     stage('Build Dcoker Image') { 
        steps { 
           sh 'docker build -t simple-app .'
        }
      }

         stage("Deploy application") { 
         steps { 
           sh 'docker run -d -p 80:80 simple-app'
         }

     }
  
   	}

   }
