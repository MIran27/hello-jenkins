pipeline {
        agent any
 stages{
   stage("rollback") {
   steps{
             git url: "ssh://jenkins@github.com/MIran27/hello-jenkins.git",
             credentialsId: '3d29306f-01ac-4fbd-92c6-0d8280ca1c66',
             branch: master

             sh 'echo $USER'
             sh 'pwd'
             sh 'ls'
             sh 'git log'
             sh 'git checkout master'
	     sh 'git pull'

             sh    'git push https://${GIT_CREDS_USR}:${GIT_CREDS_PSW}@github.com/MIran27/hello-jenkins.git master'
             
    }
    }
   

}
}
