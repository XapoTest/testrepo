pipeline {
     agent any
     triggers {
        cron('H */4 * * 1-5')
     }
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
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-15'
                 }
                 }
             
         }
     }
 }
