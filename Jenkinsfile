pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=first-app-test -Dsonar.organization=first-app-test_test1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=${{ secrets.TOKEN }}'
			}
        } 
  }
}
