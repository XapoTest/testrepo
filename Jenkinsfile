pipeline {
     agent any
     triggers {
        pollSCM '* */5 * * *'
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
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-25'
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-26'
                     jiraSendBuildInfo site: 'xapo.atlassian.net', branch: 'SATP-29'
                    
                 }
                 }
             
         }
     }
 }
