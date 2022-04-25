pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/ramdevops03/maven-build.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package -f pom.xml'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy our code in Dev or Prod'
            }
        }
    }
}
