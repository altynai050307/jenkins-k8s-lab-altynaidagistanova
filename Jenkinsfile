pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
               
                sh '''
                 
                    helm repo add microservices https://anshelen.github.io/microservices-deploy/
                    
                  
                    helm repo update
                    
                
                    helm upgrade --install demo microservices/microservices-deploy --namespace demo --create-namespace
                '''
            }
        }
    }
}
