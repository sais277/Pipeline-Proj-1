pipeline {
    agent { label 'master' }
    stages {
        stage('Buzz Build') {
            steps {
                echo "Fluffy Build Stage"
		sh 'cd $(pwd)/first/'
		sh 'python $(pwd)/first/hello.py'
            } 
        }
        stage('Fluffy Test') {
          steps {
            sh "cd $(pwd)/target'
	    archiveArtifacts(artifacts: '$(pwd)/target/*.txt', fingerprint: true)
	    echo "Test Done"
            }
        }
	stage('Fluffy Deploy') {
	  steps {
	    echo "Fluffy Deploy Done"
	    }
	}
    }
}
