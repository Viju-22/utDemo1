pipeline
{
    agent any
    
    stages{
    
        stage('Build Application'){
        steps{
        bat 'mvn -X -B -U -e -V clean install -DskipTests'
        }	
        }
        
        stage('Munit Testing'){
        steps{
        bat 'mvn clean test'
        }     
        }
             
        stage('Deploy Application To Mulesoft'){
        steps{
        bat 'mvn package deploy -DmuleDeploy -Danypoint.userName=OssomVictory4 -Danypoint.password=Capg@1999'
        }
       
        }
       
   
    }
}
