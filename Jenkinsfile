
String stringParser(String inputString) {
    inputString.split("/")[0]
}


pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo stringParser(BRANCH_NAME)
            }
        }
        stage('Test') {
            steps {
                echo 'Pouete pouete'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Cleanup') {
            when { branch "release/*" }
            steps{
                echo 'We are REALEASING ALL THE THINGS'
            }
        }
    }
}
