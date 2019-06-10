node {
    env.Java_HOME= tool name: 'MyJDK', type: 'jdk'
    def mvnHome=tool name: 'Mymaven', type: 'maven'
    def mvnCMD="${mvnHome}/bin/mvn"
  
   stage('Preparation') { 
     
     git 'https://github.com/kbprabhukumar/SeleniumMaven.git'
     
   }
   stage('Build') {
       
       script{
        echo "Compiling the code"
        bat "${mvnCMD} test"
       }
      
   }
 
}
