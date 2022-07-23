pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automationg-prod'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage prod'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Stage prod'
            }
        }

    }
}
