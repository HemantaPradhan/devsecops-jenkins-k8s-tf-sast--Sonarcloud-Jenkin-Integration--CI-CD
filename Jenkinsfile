pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-test1 -Dsonar.organization=devsecops-test1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7f75c2d94ae20c50578dc3753c20eb8b8437b423'
			}
        } 
  }
}
