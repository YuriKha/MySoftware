pipeline {
    agent any
    stages {
        stage('clone the MySoftware project:') {
            steps {
                bat 'git clone "https://github.com/YuriKha/MySoftware.git"'
            }
        }
        stage('Run MySoftware Script') {
            steps {
                script {
                    echo "Running main.py on master branch in MySoftware..."
                    bat 'python main.py'
                }
            }
        }
    }
}