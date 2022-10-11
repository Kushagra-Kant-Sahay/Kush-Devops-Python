pipeline {
    agent any
    stages {
        stage('build') {
            steps {
              echo "buildapp"        
            }
        }
       stage('test') {
            steps {
               echo "testapp"
            }
            }
        stage('deploy') {
            steps{
                echo "deployapp"
            }
        }
    }
            
            post {
                always
                {
                   // mail body: 'Pipeline was triggered build tested and code has no error woohhlaahhh', from: 'trickygyan818@gmail.com', subject: 'Pipeline Triggered', to: 'diksha1999tripathi@gmail.com'
                }
            }
        }
