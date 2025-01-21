pipeline {
    agent any
    
    stages {
        // Step 1: Clone the Repository
        stage('Clone Repository') {
            steps {
                // Pull the latest code from the GitHub repository
                git branch: 'master', url: 'https://github.com/kradars/jenkinsTrialRepo.git'
            }
        }
        
        // Step 2: Deploy the index.html file
        stage('Deploy HTML File') {
            steps {
                sh '''
                # Deploy index.html to the web server directory (e.g., /var/www/html)
                cp index.html /var/www/html/
                '''
            }
        }
    }
}
