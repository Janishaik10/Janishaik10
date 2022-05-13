pipeline {
   agent any
   tools {
        maven 'M2_HOME'
        jdk 'JAVA_HOME'
   }
   stages  {
     stage("Checkout Code from SCM GITHUB')
        steps {
          git branch: 'master',
          url: "https://github.com/pvenkatesh2291/Hello-World.git"
        }
     } 
     stage("Building Application Using MVN")  {
        steps {
        sh "mvn clean packages"
        }
     }
   }
} 
