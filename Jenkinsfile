pipeline {
	agent any
    stages {
        stage('Build on k8s ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install first-release ekscluster  --set image.repository=registry.hub.docker.com/shohagict/ekscluster --set image.tag=15'
              			
            }           
        }
    }
}
