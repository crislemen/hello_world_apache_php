pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
             sh 'docker build -t hello_world_apache_php .'
             sh 'docker run -p 8082:80 hello_world_apache_php'
            }
        }
}
}