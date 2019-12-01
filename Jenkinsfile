pipeline {
    agent any 
    stages {
        stage('clean') { 
            steps {
              echo "RMDIR /Q/S my-app"
              echo "git clone https://github.com/acehao94/my-app.git"
              echo "mvn clean C:/Program Files (x86)/Jenkins/workspace/PipelineDemo/my-app"
            }
        }
        stage('Test') { 
            steps {
             echo "mvn test C:/Program Files (x86)/Jenkins/workspace/PipelineDemo/my-app"
            }
        }
        stage('Package') { 
            steps {
                echo "mvn package C:/Program Files (x86)/Jenkins/workspace/PipelineDemo/my-app"
            }
        }
    }
}
