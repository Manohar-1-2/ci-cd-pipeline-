pipeline{
    agent {
        docker {
            image 'node:lts-iron'
        
        }
    }
   stages{
    stage('install dependencies'){
        steps{
            sh 'npm install'
        }
    }
    stage('test'){
        steps{
            sh 'npm test'
        }
    }
    stage('build'){
        steps{
            sh 'npm build'
        }
    }

   } 
}