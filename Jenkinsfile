pipeline {
    agent any
    tools {
        maven 'Maven'
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
