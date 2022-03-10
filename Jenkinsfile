pipeline {
    agent any

   
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/subedishiva/Jenkins-project-.git'

                // Run Maven on a Unix agent.
                sh "ls -l"
                sh "zip test.zip  index.htm"
                sh "zip -r test.zip second.html"
                sh "zip -r test.zip third.html"
                sh "ls -al "

                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }

                    }
    }
}
