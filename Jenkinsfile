pipeline
{
   agent any
	stages
	{
		stage('Build')
		{
		  steps
		   {
			echo "START JENKINS"
			sh 'mvn clean package'
			echo "END JENKINS"
			sh "docker build . -t MavenProjectGit:${env.BUILD_ID}" 
			echo "COMPLETE JENKINS"
		   }
		}
	}	
}
