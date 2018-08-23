pipeline {
	agent any
	stages {
		stage('Build'){
			steps {
				//echo "Hello World"
				bat 'mvn clean package'
				}
			
			post{
				success{
					
				archiveArtifacts artifacts : "**/*.war"
			}
		}
          }
    }

}
