pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/pradeepTechStream/JenkinProject.git'
            }
        }
        stage('Build') {
             steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
