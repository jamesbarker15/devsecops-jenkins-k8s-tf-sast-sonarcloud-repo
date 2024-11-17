pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_7'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jamesbarker -Dsonar.organization=jamesbarker -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=5176e2cef395b927d2ad6aff278d93aecb10383d'
			}
        } 
  }
}
