node{
	stage('SCM Checkout'){
	git'https://github.com/rajashekar45/my-app'
	
	}
	
	stage('Compile-Package'){
	def mvnHome = tool name: 'maven-1', type: 'maven'
	sh "${mvnHome}/bin/mvn clean package"

	}
	
	stage('Email-Notification'){
	mail bcc: '', body: '''Hi Team,
	These mail regarding jenkin-job

	thanks,
	Reddy ''', cc: '', from: '', replyTo: '', subject: 'jenkins-job', to: 'svsreddy.aws@gmail.com'
	
	}

}
