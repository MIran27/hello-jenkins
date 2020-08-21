pipeline {
        agent any
 stages{
   stage("rollback") {
   steps{
             
             sh 'git checkout feature/miran'
	     sh 'git revert  --no-edit ${HASH_VALUE} '
             sh 'git push https://${GIT_CREDS_USR}:${GIT_CREDS_PSW}@github.com/MIran27/hello-jenkins.git master -u origin f1/miran'
             
    }
    }
   

}
}
