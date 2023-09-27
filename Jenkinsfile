pipeline {
  agent any
  tools { 
        maven 'maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asg-buggywebapp -Dsonar.organization=asg_buggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=69bffaa2e9797272a88e2c10805d215b97386f26'
			}
        } 
  }
}
