pipeline {
   agent {
      docker {
           image 'maven:3-alpine'
	   args '-v /root/.m2:/Users/i351852/.m2' 
	}
   }
   stages {
	stage('Build') {
	  steps {
	    sh 'mvn  -B -DskipTests clean package'
	   }	
	}

   }
}
