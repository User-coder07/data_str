pipeline{
    agent any
    environment{
        JAVA_HOME = "C:/Program Files/Java/jdk-21"
        PATH = "${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages{
        stage("cloning"){
            steps{
                git url: 'https://github.com/User-coder07/data_str.git' , branch: 'main'
            }
        }
        stage("compile"){
            steps{
                bat 'javac Additions.java'
            }
        }
        stage("run java"){
            steps{
                bat 'java Additions'
            }
        }
    }
}
