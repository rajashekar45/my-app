node{
	stage('SCM Checkout'){
	git'https://github.com/rajashekar45/my-app'
	
	}
	
	stage('Compile-Package'){
	def mvnHome = tool name: 'maven-1', type: 'maven'
	sh "${mvnHome}/bin/mvn package"

	}

}
