pipeline{
    agent any

    stages{
        stage('SCM'){
            steps {
                checkout scm
            }
        }
    }

    stages{
        stage('SAST'){
            steps {
                sh 'HolaMundo'
            }
        }
    }

}