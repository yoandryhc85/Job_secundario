pipeline{
    agent any
    stages{
        
        stage('Job secundario de test'){
            
            steps{
                sh "mkdir -p output"
                writeFile file : "output/somefile", text: "Production"
                stash name: 'first-stash', includes: 'output/*' 
                echo "Esto es una prueba"
            }
        }
 
        
        
    }
   
 }
