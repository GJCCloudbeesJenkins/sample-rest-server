pipeline {
   agent any

   options {
      buildDiscarder(logRotator(numToKeepStr:'10'))
   }

   stages {
      stage('Build') {
         steps {
            sh 'echo Joe'
         }
      }
stage('Development Tests') {
         when {
            beforeAgent true
            branch 'development'
         }
         steps {
            echo "Run the development tests!"
         }
      }
   }
}
