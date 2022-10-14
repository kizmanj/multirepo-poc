pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Chekcing out repos..'
                dir('fineract') {
                    sh 'pwd'
                    sh 'ls -la ../'
                    git branch:'develop', url:'https://github.com/apache/fineract.git'
                }
                dir('mifosx') {
                    sh 'pwd'
                    git branch:'develop', url:'https://github.com/openMF/mifosx.git'
                }
                sh 'ls -la'
                sh 'ls -la fineract'
                sh 'ls -la mifosx'
           }
        }
    }
}
