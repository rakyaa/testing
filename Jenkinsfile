pipeline
{
 agent any
 stages{
    stage('Build Application'){
    steps{
    withMaven(maven : 'maven_online'){
    bat 'mvn -B -U -e -V clean -DskipTests package'
    }
   }
   } 
    stage('Deploy Application To Mulesoft Cloudhub'){
    steps{
    withMaven(maven : 'maven_online'){
    bat 'mvn deploy -DmuleDeploy'
    }
   }
   }
}

} 
 
