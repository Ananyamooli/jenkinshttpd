pipeline {
    agent any
    environment {
        MY_SECRET_PASSWORD = credentials(id)
    }
    parameters {
        string (name: 'NAME', defaultvalue: 'anu',description: 'Name of the person')
        text (name: 'PARA', defaultvalue:'',description:'Enter highlevel fixes for release')
        booleanParam (name:'TOOGLE', defaultvalue: true,description: 'would you like to scan')
        password (name: 'SECRET', defaultvalue:'SECURE PASSWORD',description:'Enter the password')
        choice (name: 'ENV',choices: ['dev','test','prod'],description: 'Which ENV would you like to deploy')
            }
    stages {
        stage ('paramaters example') {
            steps {
                echo "welcome ${params.NAME}"
                echo "fixes done are:${params.PARA}"
                echo "deploying to ${params.ENV}"
                echo "are scans happening :${params.TOOGLE}"
                echo "you entered the password as :${MY_SECRET_PASSWORD_PSW}"
            }
        }
    }
}
