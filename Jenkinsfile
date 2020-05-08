//declarative pipeline
pipeline {
    agent any
    stages{
        stage ('Build'){
        steps{
            echo "Build is running"
        }
    }
    stage ('Test'){
        steps {
            echo "Test is happenning"
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