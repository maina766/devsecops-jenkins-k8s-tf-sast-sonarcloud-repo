pipeline {
  agent any
  tools { 
        maven 'maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asg-buggywebapp -Dsonar.organization=asg-buggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=cbf151bc64d0dd344fe84705a075df23926afdb1'
			}
        } 
  }
}
