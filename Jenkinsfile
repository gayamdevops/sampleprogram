node {

   stage('SCM') {
      // git clone
	  git 'https://github.com/gayamdevops/sampleprogram.git'
   }
   
   stage ('build the packa:Wges') {
      // mvn package
	  sh 'mvn package'
   }

   
   
   stage ('archival') {
     // archiving artifacts
	 archive 'gameoflife-web/target/*.war'
   }
   stage('test results'){
   junit 'gameoflife-web/target/surefire-reports/*.xml'
}
