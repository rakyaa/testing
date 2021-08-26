	 
pipeline
{
 agent any
 stages{
    stage('Build Application'){
    steps{
    bat 'mvn -B -U -e -V clean -DskipTests package'
   }
   } 
    stage('Deploy Application To Mulesoft Cloudhub'){
    steps{
    bat 'mvn deploy -DmuleDeploy'
   }
   }
}

} 
 
