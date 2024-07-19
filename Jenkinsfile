pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('Build') { 
            steps {
                withMaven {
                    sh 'mvn -B -DskipTests clean package'
                }
            }
        }
    }
}
