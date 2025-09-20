pipeline{
    agent any
    stages{
        stage('SCM checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Abhinav501-eng/mavenproject1.git']])
            }
        }
        stages('compile the code'){
            steps{
                withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
                sh 'mvn compile'
                }
            }
        }
        stages('compile the code'){
            steps{
                withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
                sh 'mvn test'
                }
            }
        }
        stages('compile the code'){
            steps{
                withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
                sh 'mvn package'
                }
            }
        }
    }
}