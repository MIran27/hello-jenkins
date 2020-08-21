pipeline {
        agent any
 stages{
   stage("rollback") {
   steps{
             sh 'echo $USER'
             sh 'pwd'
             sh 'ls'
             sh 'git log'
             sh 'git checkout master'

             sh    'git push https://${GIT_CREDS_USR}:${GIT_CREDS_PSW}@github.com/MIran27/hello-jenkins.git master'

             sh 'git push'
             
    }
    }
   

}
}
