pipeline {
    agent any
    stages("Checkout"){
        steps{
            checkout scm
        }
    }
    stage("Test App") {
        steps{
            sh 'sudo npm install'
            sh 'npm index.js'
        }
    }

    stage("Build Images") {
        steps{
            sh 'npm run build'
        }
    }
       
}
