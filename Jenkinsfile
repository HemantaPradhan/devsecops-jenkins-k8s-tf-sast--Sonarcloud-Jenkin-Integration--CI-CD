pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-test1 -Dsonar.organization=devsecops-test1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=85cb78b836e0f079ae73208c8b280b9d56d86ad2'
			}
        } 
  }
}
