pipeline { agent any

stages {
    stage('Checkout') {
        steps {
            checkout scm
        }
    }
    
    stage('Build') {
        steps {
            sh 'echo "Building the application"'
            sh 'ls -la'
            // Thay thế bằng lệnh build thực tế của dự án
            // Ví dụ: sh 'npm install && npm run build'
        }
    }
    
    stage('Test') {
        steps {
            sh 'echo "Running tests"'
            // Thay thế bằng lệnh test thực tế của dự án
            // Ví dụ: sh 'npm test'
        }
    }
    
    stage('Deploy') {
        steps {
            sh 'echo "Deploying the application"'
            // Thay thế bằng lệnh deploy thực tế
            // Ví dụ: sh './deploy.sh staging'
        }
    }
}

post {
    success {
        echo 'Pipeline đã hoàn thành thành công!'
    }
    failure {
        echo 'Pipeline đã thất bại!'
    }
}
}
