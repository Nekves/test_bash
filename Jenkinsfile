pipeline {
    agent any

    //parameters {
    //   choice choices: ['1', '2', '3', '4', '5'], description: 'This is a choice', name: 'CHOICE'
    //}

    stages {
        stage('date') {
            steps {
                echo 'date to file'
                sh date.sh
            }
        }
        stage('Test') {
            steps {
                echo 'test'
            }
        }
        stage('Upload') {
            steps {
                echo 'upload'
            }
        }
    }
}
