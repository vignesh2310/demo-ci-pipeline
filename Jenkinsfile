pipeline {
    agent any
    tools {
        maven "maven3"
        jdk "java8"
    }

    stages {
        stage ('fetch code') {
            steps {
                git branch: 'ci-jenkins', credentialsId: 'git-cred', url: 'https://github.com/vignesh2310/ci-jenkins.git'
            }
        }
    }
}
