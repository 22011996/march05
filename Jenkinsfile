pipeline {
    agent {
        label 's1'
    }
    stages {
        stage("SCM") {
            steps {
                git branch: 'main', url: 'https://github.com/ramyachetty/vprofile-project.git'
                sh 'mvn clean install'
            }
        }
        stage("SHELL") {
            steps {
                git 'https://github.com/22011996/march05.git'
                sh 'bash demo.sh'
            }
        }
    }
}
