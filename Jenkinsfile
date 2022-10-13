pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		git url:'https://github.com/apache/fineract.git'
		git url:'https://github.com/openMF/mifosx.git'
		sh 'ls -la'
           }
        }
    }
}
