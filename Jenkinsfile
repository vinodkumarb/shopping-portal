pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
//       maven 'Maven 3.6.3' 
	nodejs
    }

    stages{
        stage('build'){
            steps{
                echo 'this is the build stage'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test stage'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package stage'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline code has completed execution...'
        }
        
    }
    
}
