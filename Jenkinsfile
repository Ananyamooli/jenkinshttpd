pipeline {
    agent any
    parameters {
        string(name: 'NAME', defaultValue: 'Siva',description: 'Name of the person')
        text(name: 'PARA', defaultValue:'',description:'Enter highlevel fixes for release')
        choice(name: 'ENV',choices: ['dev','test','prod'],description: 'Which ENV would you like to deploy')
        booleanParam(name:'TOOGLE', defaultValue: true,description: 'would you like to scan')
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
        
            }
    stages {
        stage ('paramaters example') {
            steps {
                echo "welcome ${params.NAME}"
                echo "fixes done are:${params.PARA}"
                echo "deploying to ${params.ENV}"
                echo "are scans happening: ${params.TOOGLE}"
                echo "Password: ${params.PASSWORD}"
                
            }
        }
    }
}
