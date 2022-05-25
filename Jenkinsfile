pipeline {
    agent any

    stages {
        stage('build') {
            steps {
               script {
				   def exitCode = powershell(returnStatus: true, script: ".\\build.ps1")
				   echo "build.ps1 exited with ${exitCode}"
			   }
            }
        }
    }
}
