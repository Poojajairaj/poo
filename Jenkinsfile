pipeline{
    agent any
    environment {
        PATH="/opt/maven/bin:$PATH"
    }
    
    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/Poojajairaj/poo.git'
            }
        }
        stage('Maven') {
            steps {
               sh  "mvn package"
            }
        }
    }
}    
