pipeline {
    agent any
    
    // parameters {
    //     booleanParam(name: 'opt1', defaultValue: false, description: '')
    //     booleanParam(name: 'opt2', defaultValue: false, description: '')
    // }

    stages {
        stage('opt 1') {
            // when {
            //     environment name: 'opt1', value: 'true'
            // }
            steps {
                sh 'printenv'
                sh "date > 1.txt"
                sh "date > 2.txt"
                minio bucket: 'evgeniy', credentialsId: '6d028197-12b4-4aee-a30a-600551441faf', excludes: '', host: 'http://185.4.72.16:9000', includes: 'date.txt, 2.txt', targetFolder: '$GIT_BRANCH'
            }
        }
        stage('opt 2') {
            when {
                environment name: 'opt2', value: 'true'
            }
            steps {
                sh 'printenv'
                sh "date > 1.txt"
                sh "date > 2.txt"
                minio bucket: 'evgeniy', credentialsId: '6d028197-12b4-4aee-a30a-600551441faf', excludes: '', host: 'http://185.4.72.16:9000', includes: 'date.txt, 2.txt', targetFolder: '$STAGE_NAME'
            }
        }
    }
}
