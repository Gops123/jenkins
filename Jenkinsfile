
pipeline{
	agent any
	stages{
  		stage('Compile Stage'){
    			steps{
      				withMaven(mave: 'maven_3_5_0'){
        				sh 'mvn claen compile'
      				}
    			}
  		}
  		stage('Testing Stage'){
    			steps{
      				withMaven(mave: 'maven_3_5_0'){
        				sh 'mvn test'
      				}
    			}
  		}
  		stage('Deployment Stage'){
    			steps{
      				withMaven(mave: 'maven_3_5_0'){
        				sh 'mvn deploy'
      				}
    			}
  		}
	}
}
