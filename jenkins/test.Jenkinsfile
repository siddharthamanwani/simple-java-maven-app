def gv

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                gv = load 'jenkins/script.dev.groovy'
                gv.load_check()
                echo "build stage"
            }
        }
        stage('Test') {
            steps {
                echo "test stage"
                gv.print_message(3)
            }
        }
    }
}
