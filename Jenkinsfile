pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asg-app -Dsonar.organization=asg-app -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=dc8cb70a84f715a996af9b418ab67c422d65dcbe'
			}
        } 
  }
}
