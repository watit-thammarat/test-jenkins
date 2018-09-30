node {
	stage('Git') {
		git 'https://github.com/gustavoapolinario/microservices-node-example-todo-frontend.git'
	}
	stage('Build') {
		sh 'npm install'
		sh 'npm run bowerInstall'
	}
	stage('Test') {
		sh 'npm test'
	}
}