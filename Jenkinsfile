//declarative scripting
pipeline {
    agent any
    stages {
        stage ('checkout'){
         steps {
             echo"checkout is done"
         }
        }
        stage ('Build'){
            steps{
                echo "Build is running"
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