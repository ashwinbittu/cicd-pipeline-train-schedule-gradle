pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automationg-stage'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage steage'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Stage stage'
            }
        }

    }
}
