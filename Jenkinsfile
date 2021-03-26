pipeline{
    agent{
        node{
            label 'agent01'
        }
    }
    options{
        buildDiscarder(logRotator(numToKeepStr: '5'))
        disableResume()
        disableConcurrentBuilds()
        timestamps()
    }
    stages{
        stage('Stage-1'){
            steps{
                sh 'sleep 2'
                sh 'echo Hello from stage-1'
            }
        }
        stage('Stage-2'){
        	sh 'sleep 2'
		sh 'echo Hello from stage-2'
        }
    }
}
