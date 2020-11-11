pipeline {
    agent { label 'master' }
    stages {
        stage('Fluffy Build') {
            steps {
                echo "Fluffy Build Stage"
		echo "pushing to Test Branch"
		sh 'pwd'
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
