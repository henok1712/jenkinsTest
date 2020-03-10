pipeline{
agent any
stages {
    stage ('build Application'){
        steps {
        
            bat 'mvn clean install'
        }
    }
    stage ('Test Application'){
        steps{
        
            bat 'mvn clean test'
        }
    }
    stage('Deploy Application'){
        steps {
    
                   bat 'mvn clean package deploy -Dmule.version=4.2.2 -Dusername=solution -Dpassword=Robert123 -Denvironment=Sandbox -Dworkers=1 -Dworker.type=Micro -Dapplication.name=capstoneJenkinsTest'
           
            }
        }
     }
 }
