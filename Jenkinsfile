pipeline {
    agent { node { label 'Agent-1' } } 

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'Webhook concept in jenkins'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }    
    post { 
          always { 
            echo 'I will always run whether the job is success or not'
            }
          success{
            echo 'I will run always when the job is success'
           } 
          failure{
            echo ' I will run always when the job fails'
           }   
    }
    
}