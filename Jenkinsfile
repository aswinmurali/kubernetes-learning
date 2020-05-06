//declarative scripting
pipeline {
    agent any
    stages {
        stage ('Build'){
         steps {
             echo"Build is done"
         }
        }
        stage ('Test'){
            steps{
                echo "Test is running"
            }
        }
       
    }
     post {
            success{
                echo "The build ran successfully"
            }
            failure{
                echo "There is a failure"
            }

        }
}