pipeline {
    agent {
        docker {
            image 'maven:3.1'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
   }
 }
}
