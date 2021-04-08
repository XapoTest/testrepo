pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 echo 'Building...'
             }
             post {
                 always {
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-11'
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-8'
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-7'
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-14'
                 }
                 }
             
         }
     }
 }
