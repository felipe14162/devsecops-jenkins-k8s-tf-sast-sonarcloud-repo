pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecgbuggywebapp -Dsonar.organization=MyOrganization -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6fe462259efa850f0f1548f1ebb4e12cedcfada6'
			}
        } 
  }
}
