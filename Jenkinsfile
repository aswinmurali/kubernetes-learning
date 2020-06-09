pipeline {
    agent any 
    environment {
        mavenHome = tool 'maven'
        PATH = "$mavenHome/bin:$PATH"
    }
    stages {
        stage  ('checkout') {
steps {
                sh 'echo "checkout is running"'
            }
        }
        stage ('compile') {
            steps {
           sh 'mvn --version'
           sh 'mvn clean compile'
            }
        }
        stage('Unit Test') {
            steps {
                sh 'mvn test'
            }
        }
        }
        post {
            sucess {
                echo "Always successful"
            }
            failure{
                echo "Your build has failed to run"
            }
        }
    }