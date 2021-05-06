pipeline{

    agent any

    tools{
       nodejs 'nodejs' 
    }

    stages{
        stage('build'){
            steps{
                echo 'Starting Build Job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'Starting Test Job'
                sh 'npm test'
//                sleep 9
            }
        }
        stage('package'){
            steps{
                echo 'Starting Package Job'
                sh 'npm run package'
//                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline is for shopping portal...'
        }
        
    }
    
}
