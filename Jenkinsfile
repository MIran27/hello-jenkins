pipeline {
        agent any
 stages{
   stage("rollback") {
   steps{
             
             sh 'git checkout f8/miran'
             sh 'git pull'
	     sh 'git revert -m 1  --no-edit ${HASH_VALUE} '
             sh 'git push https://${GIT_CREDS_USR}:${GIT_CREDS_PSW}@github.com/MIran27/hello-jenkins.git'
             
             
    }
    }
   

}
}
