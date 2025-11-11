pipeline {
    agent any

    stages {
        stage('Clone Source') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/sachin841/sparkjava-war-example.git'
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
