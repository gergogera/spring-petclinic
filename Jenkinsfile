echo 'Hello from Pipeline Demo'
stage('Compile') {
	node {
		git 'https://github.com/gergogera/spring-petclinic.git'
		def mvnHome = tool 'maven-3.3.9'
		bat "${mvnHome}\\bin\\mvn -B compile"
	}
}
