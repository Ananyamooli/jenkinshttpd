pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage('proddeploy') {
            when {
                environment name:'DEPLOY_TO', Value:'other'
            }
            steps {
                echo "deploy to production"
            }
        } 
    }
}
