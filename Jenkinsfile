node {
   stage('Preparation') {
       checkout scm;
   }
   stage('Test') {
   }
   stage('Results') {
      emailext(
         body: '${env.BUILD_LOG}',
         attachLog: true,
         subject: '${env.BUILD_ID}',
         to: 'santoshiyengar@gmail.com'
      )   
   }
}
