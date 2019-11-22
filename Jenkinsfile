pipeline {
    agent any
    tools {
        maven 'Maven'
    }
    stages {

        // stage('Initialize'){
        //         def dockerHome = tool 'mydocker'
        //         env.PATH = "${dockerHome}:${env.PATH}"
        // }

        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean install'
            }
        }
        // stage('Test') {
        //     steps {
        //         sh 'mvn test'
        //     }
        //     post {
        //         always {
        //             junit 'target/surefire-reports/*.xml'
        //         }
        //     }
        // }
        // stage('Deliver') {
        //     steps {
        //         sh './jenkins/scripts/deliver.sh'
        //     }
        // }
        //  stage('Publish') {
        //      steps {
        //         echo 'Starting to build docker image!!'

        //         script {
        //             // withDockerRegistry([credentialsId: 'puneetvashisht', url: 'docker.io/puneetvashisht']) {
        //                 def customImage = docker.build("puneetvashisht/dockerwebdemo:latest")
        //                 customImage.push()
        //             // }
                  
        //         }
        //     }
        // }
    }
}
