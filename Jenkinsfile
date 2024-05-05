pipeline {
    agent any
    stages("Checkout"){
        steps{
            checkout scm
        }
    }
    stages("Test App") {
        steps{
            sh 'sudo npm install'
            sh 'npm index.js'
        }
    }

    stages("Build Images") {
        steps{
            sh 'npm run build'
        }
    }
       
}
