pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Cloning repository from github.."
                git branch: "master", url: "https://github.com/kudratmullani/javaparser-maven-sample.git"
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
