pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                checkout scm
                sh 'printenv'
                // Clean the workspace and clone the GitHub repository
              //  deleteDir()
               // git 'remote set-url origin git@github.com/vsawanny/demo-devops.git'
                //git 'https://github.com/vsawanny/demo-devops.git'
            }
        }
        stage('Build and Run Java') {
            steps {
                // Assuming the Java file is located at the root of the repository
              //  dir("${env.WORKSPACE}") {
                    sh 'javac test.java' // Compile the Java file
                    sh 'java HelloWorld'       // Run the Java program
               // }
            }
        }
    }
}
