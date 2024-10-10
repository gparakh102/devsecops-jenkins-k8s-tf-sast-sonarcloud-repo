pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=lolbuggywebapp -Dsonar.organization=lolbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=721142787e96716b20839ee344b1984a516aa4b3'
			}
        } 
  }
}
