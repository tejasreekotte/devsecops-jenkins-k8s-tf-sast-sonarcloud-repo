pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=tkbuggywebapp -Dsonar.organization=tkbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c76a708d58559a63b9db8ab7f34a6dfb0e03db85'
			}
        } 
  }
}
