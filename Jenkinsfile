pipeline {
    agent any

    //parameters {
    //   choice choices: ['1', '2', '3', '4', '5'], description: 'This is a choice', name: 'CHOICE'
    //}

    stages {
        stage('date') {
            steps {
		echo 'add webhook'
                echo 'date to file'
                sh 'env'
                sh 'pwd'
                sh 'ls -la'
                //sh 'bash ./date.sh'
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
