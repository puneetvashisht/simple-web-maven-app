pipeline {
    agent any
    tools {
        maven 'Maven'
    }
    stages {

        stage('FirstStage') {
            steps {
                // sh 'docker --version'
                echo 'Executing First Stage'
            }
        }

        stage('CreateDockerImage') {
            steps {
                sh 'mvn install -DskipTests'
            }
        }
        stage('DeployDockerImage') {
            steps {
                // sh 'docker --version'
                echo 'Starting to deploy docker image!!'
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
