pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage('proddeploy') {
            when {
                environment name:'DEPLOY_TO', Value:'production'
            }
            steps {
                echo "deploy to production"
            }
        } 
    }
}
