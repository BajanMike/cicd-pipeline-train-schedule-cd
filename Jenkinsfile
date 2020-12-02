pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running the build automation hold on'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
