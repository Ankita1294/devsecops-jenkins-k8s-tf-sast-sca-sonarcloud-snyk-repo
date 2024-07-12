pipeline {
  agent any
  tools { 
        maven 'Maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ankibuggywebapp -Dsonar.organization=ankibuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=ae83b598e7f9e4a8c35d0b780274bc21d2e22b78'
			}
    }
    }		
  }

