pipeline {
    agent {
        docker {
            image 'ubuntu'
            args '-t -d'
 stages {
    stage('Git branch to be committed') {
           steps {
              git branch: '*/*', url: 'https://github.com/dvp-2/jenkins-repo-test.git'
                //sh 'ls -al > testing1.txt' 
               // sh 'docker tag nginxtest:8 dvp1/nginx-jenkins:8'
               
          }
        }
     stage('Docker Build and Tag') {
           steps {
              
                sh 'ls -al > testing1.txt' 
               // sh 'docker tag nginxtest:8 dvp1/nginx-jenkins:8'
               
          }
        }
     
 /* stage('Publish image to Docker Hub') {
          
            steps {
          withDockerRegistry([ credentialsId: "dockerhubcred", url: "" ]) {
       
          sh  'docker push dvp1/nginx-jenkins:8' 
        }
                  
          }
        }
     
      stage('Run Docker container on Jenkins Agent') {
             
            steps {
                sh "docker run -d -p 3001:80 nginxtest:8"
 
            }
        }  */
 
    }
}
