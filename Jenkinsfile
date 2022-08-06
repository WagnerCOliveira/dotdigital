node("AWS-02-AGENT"){
    image = 'gitea/gitea'
    stage('Clean Workspace') {
        cleanWs()
    }
    stage('Clone') {
		git branch: 'step4', url: 'git@github.com:WagnerCOliveira/dotdigital.git'
		sh 'rm -rf .git'
	}
	stage ('Pull-Image'){
	    withDockerRegistry(credentialsId: 'dockerregistry', url: 'https://index.docker.io/v1/') {
            docker.image(image).pull()
        }
	}
    stage('Stack-Deploy'){
        sh 'docker-compose up -d'        
    }
}