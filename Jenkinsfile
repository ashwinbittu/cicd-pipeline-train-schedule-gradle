pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automationgbranch-2'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage branch-2'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Stage branch-2'
            }
        }

    }
}
