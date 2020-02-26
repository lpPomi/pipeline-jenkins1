
node{
 
   stage('SCM Checkout'){
     git 'https://github.com/lpPomi/pipeline-jenkins1'
   }
  
  // stage('Compile-Package'){
      // Get maven home path
     // def mvnHome =  tool name: '', type: 'maven' 
      // sh "${mvnHome}/bin/mvn package"
  //    sh "/opt/maven/bin/mvn package"
  // }

   stage('Build') {
            steps {
                sh 'mvn -B package'
            }
        }

}
