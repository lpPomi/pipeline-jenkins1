node{
 
   stage('SCM Checkout'){
     git 'https://github.com/lpPomi/pipeline-jenkins1'
   }
  
  // stage('Compile-Package'){
      // Get maven home path
      def mvnHome =  tool name: '', type: 'maven' 
       echo 'Maven Home'
       echo '${mvnHome}/bin'
      // sh "${mvnHome}/bin/mvn package"
  //    sh "/opt/maven/bin/mvn package"
  // }

   stage('Build') {
      echo 'in Stage Build...  Scripted Pipeline'
      echo 'Maven version'
      sh 'mvn -v'
      echo 'Clean maven'
      sh 'mvn clean'
      echo 'Package maven'
      sh 'mvn -B package'
   }
}


      
