pipeline {
    agent any
    stages {
        stage ('checkout source') {
            steps {
                git branch: 'master', url: 'https://github.com/shivakrishna090696/hello-world.git'
            }
        }
        stage ('to check maven version') {
            steps {
                sh 'mvn --version'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
