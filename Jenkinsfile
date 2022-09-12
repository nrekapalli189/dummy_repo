pipeline {
    agent any
    stages {
        stage('git clone'){
            steps {
                git 'https://github.com/nrekapalli189/dummy_repo.git'
            }
        }
                
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {
                branch 'production'
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}
