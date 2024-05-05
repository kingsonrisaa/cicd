pipeline {
    agent any
    stages { 
        stage("Checkout"){
         steps{
             checkout scm
        }
    }
        stage("Test App") {
            steps{
                sh 'npm install'
                sh 'npm index.js'
        }
    }
 
}
}
