pipeline {
    agent any
    triggers {
        // GitHub webhook triggers the pipeline on every commit
        githubPush()
    }
    stages {
        stage('Clone Repository') {
            steps {
                // Change to the correct branch name, e.g., 'main' or 'master'
                git branch: 'main', url: 'https://github.com/NageenaS/Stress_Testing.git'
            }
        }
    }
}
