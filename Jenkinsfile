pipeline {
  agent any
  tools { 
        maven 'mvn_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-skukreja -Dsonar.organization=devsecops-skukreja -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c'
			}
        } 
  }
}
