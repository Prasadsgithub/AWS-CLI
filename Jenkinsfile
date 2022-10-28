pipeline {
    agent any
    stages {
        stage('sourcecode') {
            steps {
                git url:'https://github.com/Prasadsgithub/AWS-CLI.git',
                branch: 'main'
            }
        }
        stage(caling AWSCLI) {
            steps {
                sh "chmod +x -R ${env.WORKSPACE}"
                sh './awscli.sh'
            } 
        }
    }
}
    