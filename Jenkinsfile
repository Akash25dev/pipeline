pipeline{
   agent any
         stages{
            stage(clone){
                   steps{
                     git 'https://github.com/Akash25dev/pipeline.git'
                   }
            }
            stage(build){
                   steps{
                     sh '/home/akash/Documents/Maven/apache-maven-3.8.8/bin/mvn install'
                   }
            }
            stage(deploy){
                   steps{
                     sh 'cp target/pipeline.war /home/akash/Documents/Maven/apache-tomcat-9.0.93/webapps'
                   }
            }
        }
}

