pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('-----Build-----') { 
            steps { 
                sh 'sudo ls /var/lib/jenkins/workspace/'
            }
        }
        stage('-----Test-----'){
            steps {
                sh 'sudo javac HelloWorld.java'
                sh 'sudo touch /root/khoa.txt'
            }
        }
        stage('-----Deploy-----') {
            steps {
                sh 'echo "khoa"'
                sh 'sudo java HelloWorld'
            }
        }
    }
}
