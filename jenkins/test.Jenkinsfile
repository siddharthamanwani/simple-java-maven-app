def gv

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    gv = load 'jenkins/script.dev.groovy'
                    echo "build stage"
                    gv.load_check()
                    echo "build stage 2"
                }
            }
        }
        stage('Test') {
            steps {
                echo "test stage"
                //gv.print_message(3)
            }
        }
    }
}
