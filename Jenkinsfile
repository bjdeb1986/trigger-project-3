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
        stage('Test'){
            steps{
                sh 'sleep 2'
                sh 'echo Hello World'
            }
        }
    }
}
