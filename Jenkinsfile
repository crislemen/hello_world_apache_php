pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
             sh 'git clone'
             sh 'sudo docker build -t HELLO_WORLD_PHP_APACHE'
             sh 'sudo docker run -p 8082:80 HELLO_WORLD_PHP_APACHE'
            }
        }
}
