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
	    archiveArtifacts(artifacts: 'target/*.tgz', fingerprint: true)
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
