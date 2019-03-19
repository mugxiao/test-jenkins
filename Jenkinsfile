pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                which singularity
                //singularity build Singularity.simg Singularity
            }
        }
        stage('Test') {
            steps {
                which docker
                //singularity exec Singularity.simg python -V
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}