@Library('Jenkins-shared-lib') _
pipeline{
    agent any
    stages{
        stage('Git checkout'){
            steps{
                gitCheckout(
                    branch: 'main',
                    url: 'https://github.com/NIBI23/Jenkins-shared-lib.git'
                    
                )
            }   
        }

        stage('unit test'){
            steps{
                mvnTest()
            }   
        }
    }
}