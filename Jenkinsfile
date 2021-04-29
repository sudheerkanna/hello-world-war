pipeline {
    agent any
    environment {
        PATH= "/usr/share/maven/bin/:$PATH"
    }
    stages {
        stage('fetch code from github') {
            steps {
                git 'https://github.com/nihaldevops/hello-world-war.git'
            }
        }
        stage('build package') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
