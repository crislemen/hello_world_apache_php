pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
             sh 'docker build -t HELLO_WORLD_PHP_APACHE'
             sh 'docker run -p 8082:80 HELLO_WORLD_PHP_APACHE'
            }
        }
}
}