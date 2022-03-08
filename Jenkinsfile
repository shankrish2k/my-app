node{
   stage('SCM Checkout'){
     git 'https://github.com/shankrish2k/my-app.git'
   }
   stage('Compile-Package'){

      def mvnHome =  tool name: 'maven3', type: 'maven'   
      sh '/opt/apache-maven-3.8.4/bin/mvn clean package'
	  sh 'mv target/myweb*.war target/newapp.war'
   }
}
