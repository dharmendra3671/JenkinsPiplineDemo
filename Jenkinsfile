pipeline {
    agent any

    stages {
       stage('Wait for user to input text?') {
    steps {
        script {
             bat 'posnegint.py'
            // Define Variable
             def USER_INPUT = input(
                    message: 'Enter number to find list of positive and negative number.',
                    parameters: [
                            [$class: 'GlobalVariableStringParameterDefinition',
                             name: 'input',
                             description: 'taking user inputs']
                    ])

            echo "The answer is: ${USER_INPUT}"
            }
        }
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
