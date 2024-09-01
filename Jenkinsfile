pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testapp1_testapp1 -Dsonar.organization=testapp1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=XXXXXX'
			}
        } 
  }
}
