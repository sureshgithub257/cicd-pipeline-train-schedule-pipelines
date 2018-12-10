pipeline {
	agent any 
		stages {
			Stage('Build') {
				step {
				  echo 'Running Build automation'
				  sh './gradlew build --no-deamon'
				  archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
