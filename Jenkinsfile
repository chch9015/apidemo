pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                git branch: 'develop', url: 'https://github.com/chch9015/apidemo.git'
            }
        }
        stage('deploy to the server'){
            steps{
                sh 'scp /var/lib/jenkins/workspace/dev-apideploy/helloworld.py root@10.1.3.87:/opt/'
            }
        }
    }
}