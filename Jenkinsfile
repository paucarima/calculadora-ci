pipeline { 
    agent any 
    stages { 
        stage('Checkout') { 
            steps { 
                checkout scm 
            } 
        } 
        stage('Install Dependencies') { 
            steps { 
                sh 'npm install' 
            } 
        }
stage('Lint') { 
steps { 
sh 'npx eslint calculator.js' 
} 
} 
} 
post { 
always { 
cleanWs() 
} 
} 
} 