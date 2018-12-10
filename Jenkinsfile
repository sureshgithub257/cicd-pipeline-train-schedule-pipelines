pipeline {
	agent any {
		stages {
			Stage('Build') {
				echo 'Building the code'
				sh './gradlew build --no-deamon'
				archieveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
