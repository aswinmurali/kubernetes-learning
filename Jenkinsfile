//declarative pipeline
pipeline {
    //agent any
    agent {docker {image 'maven:3.6.3'}}
    stages{
        stage ('checkout'){
        steps{
            echo "checkout is running"
        }
    }
    stage ('Build'){
        steps {
            sh 'echo "The maven version is " $(mvn --version)'
        }
    }
}
post{
    always{
    echo "always run"
    }
    success{
    echo "sucessful"
    }
    failure{
    echo "failure"
    }
}
}