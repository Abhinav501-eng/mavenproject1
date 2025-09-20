pipeline{
    agent any
    stages{
        stage('SCM checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Abhinav501-eng/mavenproject1.git']])
            }
        }
        stage('code compilation'){
        steps{
            withMaven(jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', traceability: true) {
          sh 'mvn compile'
        }
                }
        }
}
}