pipeline {
    agent any

    stages {
        stage('build'){
            steps {
            git 'https://github.com/cjuttika/SpbootDockerJenkins.git'
            sh ‘./mvnw compile'
                echo 'Maven build successfull'
            }
        }
         stage('Test'){
            steps {
            sh ‘./mvnw test'
                echo 'Testcases executed successfull'
            }
        }
        stage('package'){
            steps {
            sh ‘./mvnw package'
                echo 'Testcases executed successfull'
            }
        }
         stage('Deploy'){
            steps {
                echo 'deploy build successfull'
            }
        }
        
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}