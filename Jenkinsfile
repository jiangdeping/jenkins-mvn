pipeline {
    agent any
    tools {
        maven 'mvn-3.5.4'
    }

    stages {
        stage('git clone'){
            git credentialsId: '9b782c00-9158-4034-b88b-b57390a5eda0', url: 'git@github.com:jiangdeping/jenkins-mvn.git'

    }

        stage('Build'){
            steps{
             //   sh "mvn clean package spring-boot:repackage"
                sh "printenv" //将环境变量打印到console中
                echo "Running $env.BUILD_NUMBER on $env.JENKINS_URL"
                }
        }
    }
}