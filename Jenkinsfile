pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                sh '''
                    withAWS(credentials:'aws-static') {
                        s3Upload(file:'index.html', bucket:'udacity-jaepaek-cloud-devops-jenkins-proj')
                    }
                '''
            }
        }
    }
}
