pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
             sh 'docker build -t hello_world_apache_php .'
             sh 'docker run -d 8082:80 hello_world_apache_php'
            }
        }
        stage('Test'){
            steps{
                sh 'wget http://localhost:8082/'
            }
        }
}
}