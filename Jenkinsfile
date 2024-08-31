pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=first-app-test -Dsonar.organization=first-app-test_test1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=d51e730f3332020ea58950d8b566d305c4ef1cab'
			}
        } 
  }
}
