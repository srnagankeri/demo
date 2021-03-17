pipeline{
	agent any
	  stages{
			stage ('one'){
				steps{
				 echo 'hi, this is edureka'
				}
			}
			
			stage('two'){
				steps{
					input('do you want to proceed?')
				
				}
			
			}
		  
		  			stage('three'){
				parallel{
				         stage('unit test'){
				              steps{
				            echo 'running UT'
				}
				       }
				stage('integration test'){
				         
				      steps{
				   echo 'running IT'
				}
				   }
				}
					}

			 
			
						
			
			
			}
}

