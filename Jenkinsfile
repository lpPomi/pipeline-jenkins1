pipeline {
node{

   agent any
   

    stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }

   stage('SCM Checkout'){
     git 'https://github.com/lpPomi/pipeline-jenkins1'
   }
   stage('Compile-Package'){
      // Get maven home path
     // def mvnHome =  tool name: '', type: 'maven' 
      // sh "${mvnHome}/bin/mvn package"
      sh "/opt/maven/bin/mvn package"
   }

}
}