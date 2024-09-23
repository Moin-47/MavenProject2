pipeline{
	agent any
		stages{
			stage("validate"){
				steps{
					echo "checking for pom.xml file"
					bat 'mvn validate'
				     }
				         }
			stage("build"){
				steps{
					bat 'mvn clean package'
				     }
				      }
	 		stage("test"){
				steps{
					bat 'java -jar MavenProject-0.0.1-SNAPSHOT.jar'
			             }
		   		     }
		 	}
	}		
					
