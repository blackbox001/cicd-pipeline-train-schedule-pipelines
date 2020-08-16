pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                ///sh './gradlew build --no-daemon'
                sh '''
                ./gradlew build --no-daemon
                echo "Finished"
                '''
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
