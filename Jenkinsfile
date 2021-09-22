pipeline {
    agent any
    environment {
        PATH = "/usr/share/man/man1:$PATH"
    }
    stages {
        stage("clone"){
            steps{
               git credentialsId: 'credential', url: 'https://github.com/Fajar-Aminul/hello-world.git'
            }
        }
        stage("build"){
            steps{
              sh "mvn clean install"
            }
        }
        
    }
}
