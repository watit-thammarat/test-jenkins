node {
	tools {nodejs "node"}
	
	stage('Git') {
		git 'https://github.com/watit-thammarat/test-jenkins'
	}
	stage('Build') {
		sh 'npm install'
		sh 'npm run bowerInstall'
	}
	stage('Test') {
		sh 'npm test'
	}
}