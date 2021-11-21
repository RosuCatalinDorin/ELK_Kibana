  pipeline {
   agent any
      stages {
         steps {
            git branch: 'master',
                credentialsId: 'GitHubCataRosu',
                url: 'https://github.com/RosuCatalinDorin/ELK_Kibana.git'

            sh "ls -lat"
            sh "cp /var/lib/jenkins/workspace/ELK_Kibana /opt"
        }
          stage("build") {
            steps {
              echo 'bulding the application'
            }
          }
           stage("test") {
            steps {
              echo 'testing the application'
            }
          }
              stage("deploy") {
            steps {
              echo 'deploying the aplication'
            }
          }
     }
  }
