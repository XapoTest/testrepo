pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 echo 'Building...'
             }
             post {
                 always {
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-8'
                 }
             }
         }
     }
 }
