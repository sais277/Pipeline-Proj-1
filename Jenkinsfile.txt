pipeline {
    agent { label 'master' }
    stages {
        stage('Fluffy Build') {
            steps {
                echo "Fluffy Build Stage"
            } 
        }
        stage('Fluffy Test') {
          steps {
            echo "Fluffy Test Done"
            }
        }
	stage('Fluffy Deploy') {
	  steps {
	    echo "Fluffy Deploy Done"
	    }
	}
    }
}
