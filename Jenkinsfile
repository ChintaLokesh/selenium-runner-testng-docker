pipeline
{
   agent any 
   stages
   {
     stage("pull the latest Image")
	   {
            steps
		   {
			   bat "docker pull chintalokesh/selenium-docker"
		   }   
	   }
     stage("Start the Grid")
	 {
	   steps
	   {
	     bat "docker-compose up -d hub chrome"
	   }
	 }
     stage("Run Test")
	 {
	   steps 
	   {
	     bat "docker-compose up Execute"
	   }
	 }
   }
	post{
		always{
			archiveArtifacts artifacts: 'output/**'
			bat "docker-compose down"
		}
	}
   
}
