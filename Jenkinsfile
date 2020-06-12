node {

   stage('SCM') {
      // git clone
	  git 'https://github.com/gayamdevops/sampleprogram.git'
   }
   
   stage ('build the packages') {
      // mvn package
	  sh 'mvn package'
   }

   
   
   stage ('archival') {
     // archiving artifacts
	 archive 'gameoflife-web/target/*.war'
   }

}
