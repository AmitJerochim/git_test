pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
								sh 'echo helloWorldfrombash'
								sh 'pwd'
								sh 'ls -la'
								sh 'bash test.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
		POST {
			always {
				echo 'i am always executed'
			}

			success {
				echo 'built, tested and deployed successfully'
			}

			failure {
				echo 'something went bad'
			}
		}
}
