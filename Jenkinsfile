pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggyweb -Dsonar.organization=buggywebapp -Dsonar.host.url=https://github.com/maina766/terraform-ec2-jenkins-aws-k8s-infra-creation.git 	'
			}
        } 
  }
}
