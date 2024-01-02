pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=azuredevopsadodevsecopsprojectkey -Dsonar.organization=azuredevopsdevsecopsoorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=294bd7d3d9c003d335e5774a736881859a9085b5'
			}
        } 
  }
}
