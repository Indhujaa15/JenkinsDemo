pipeline {
    agent any

    stages {
        stage('Fetch code') {
            steps {
                git branch: 'main', url: 'https://github.com/Indhujaa15/JenkinsDemo.git'
            }
        }
        stage('Install apache') {
            steps {
                sh 'sudo apt install apache2 -y'
            }
        }
        stage('Deploy App') {
            steps {
                sh 'sudo cp -R * /var/www/html/'
            }
        }
    }
}
