//declarative pipeline
pipeline {
    agent any
    environment {
        dockerHome = tool 'docker'
        mavenHome = tool 'maven'
        PATH = $dockerHome:/bin/mavenHome/:$PATH 

    }
    //agent {docker {image 'maven:3.6.3'}}
    stages{
        stage ('checkout'){
        steps{
            echo "checkout is running"
        }
    }
    stage ('Build'){
        steps {
            sh 'echo "The Java version is " $(java -version)'
            sh 'echo "The maven version is " $(maven -version'
            echo "Build number - $env.BUILD_NUMBER"
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
