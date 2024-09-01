pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsbuggywebapplication -Dsonar.organization=devsecopsbuggywebapplication -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=404c00e0d0f7def97b915dbba0fd0e3435870bb2'
			}
        } 
  }
}
