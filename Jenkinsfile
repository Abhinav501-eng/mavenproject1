pipeline{
    agent any
    stages{
        stage('SCM checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Abhinav501-eng/mavenproject1.git']])
            }
        }
        /*stage('compile the code'){
            steps{
                withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
                sh 'mvn compile'
                }
            }
        }
        stage('test the code'){
            steps{
                withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
                sh 'mvn test'
                }
            }
        }
        stage('build the code'){
            steps{
                withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
                sh 'mvn package'
                }
            }
        }*/
    }
}