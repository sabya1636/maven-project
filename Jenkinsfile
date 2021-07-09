node {
	stage('SCM') {
		git 'https://github.com/sabya1636/maven-project.git'
	}
	
	stage('build the package') {
		sh 'mvn clean package'
	}
	
	stage('archival') {
		archive 'server/target/*.jar'
	}
}