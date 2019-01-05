node {
   stage('SCM') {
       // git clone
       git "https://github.com/asquarezone/game-of-life.git"
       
   }
   stage('build the packages') {
       //mvn package
       sh 'mvn package'
   }
   stage ('archival') {
       // aarchiving artifacts
       archiveArtifacts 'gameoflife-web/target/*.war'
   }
}
