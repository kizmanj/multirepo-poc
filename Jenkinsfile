pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Chekcing out repos..'
		dir('fineract') {
			git url:'https://github.com/apache/fineract.git'
		}
		dir('mifosx') {
			git url:'https://github.com/openMF/mifosx.git'
		}
		sh 'ls -la'
           }
        }
    }
}
