pipeline {
    agent { label 'master' }
    stages {
        stage('Buzz Build') {
            steps {
                echo "Fluffy Build Stage"
		sh 'cd $(pwd)/first/'
		sh 'python hello.py'
            } 
        }
        stage('Fluffy Test') {
          steps {
            sh "sleep 10"
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
