pipeline{
    agent any

    stages{
        stage('SCM'){
            steps {
                checkout scm
            }
        }

        stage('SAST'){
            steps {
                sh 'chmod +x gradlew'
                sh './gradlew sonarqube -Dsonar.login=2ae30d5987686cf2c4024bdc9945b2ef9c553974 -Dsonar.branch.name=feature-lab4'
            }
        }
    }
}

