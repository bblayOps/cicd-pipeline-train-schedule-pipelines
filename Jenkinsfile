pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'Run build!!!'
                sh './gradlew build'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true
            }      
        }
    }
}
