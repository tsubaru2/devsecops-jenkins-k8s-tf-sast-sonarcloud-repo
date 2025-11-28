pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=tsubaru2 -Dsonar.organization=tsubaru2 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=57c3b8e2b4dab060726a3cda93cc2faadb5853d7'
			}
        } 
  }
}
