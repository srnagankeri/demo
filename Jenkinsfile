Pipeline{
	Agent any
	  stages{
			Stage ('one'){
				Steps{
				 echo 'hi, this is edureka'
				}
			}
			
			Stage('two'){
				Steps{
					Input('do you want to proceed?')
				
				}
			
			}
			 
			Stage('three'){
				When {
					Not {
						Branch "master"
					}
				
				}
				Steps{
					Echo 'hello'
				}
			}
			
			Stage('four'){
				Parallel{
				         stage('unit test'){
				              steps{
				            echo 'running UT'
				}
				       }
				Stage('integration test'){
				         
				      agent {
				               docker{
				                      reuseNode false
				                    image 'ubantu'
				             }
				       }
				  steps{
				   echo 'running IT'
				}
				   }
				
				
				
				}
				 
				
				
				}
			
			
			
			}
			
	
	}
}

