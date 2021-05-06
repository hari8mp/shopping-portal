pipeline{

    agent any

    tools{
       nodejs ‘nodejs’ 
    }
    

    stages{
        stage(‘build’){
            steps{
                sh ’npm install’
            }
        }
        stage('test'){
            steps{
                sh ‘npm test’
            }
        }
        stage(‘package’){
            steps{
                sh ‘npm run package’
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline for shopping-portal is completed...'
        }
        
    }
    
}
