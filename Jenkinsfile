pipeline{
 agent any
 tools{
     maven 'Maven3.6.3'
 }
 stages{
     stage("CheckOut"){
         steps{
             git branch: 'J2EE', url: 'https://github.com/ChandraSekharAlla/onlinebookstore.git'
         }
     }
     stage("build"){
         steps{
             sh 'mvn clean package'
         }
     }
 }
}
