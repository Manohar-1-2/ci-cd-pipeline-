pipeline{
   agent {
    label 'agent'
   }
   stages{
    stage('git pull'){
        steps{
            git 'https://github.com/monicatvera/2048'
        }
    }
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