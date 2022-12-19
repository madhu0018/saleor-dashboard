pipeline{
    agent {label {label 'WORKSHOP'}}
    stages{
        stage('vcs') {
            steps{
                git url: 'https://github.com/madhu0018/saleor-dashboard.git' ,
                branch : 'main'
            }
        }
            stage('Docker build') {
              steps{  
                 sh 'docker image build -t saleordashboard:1.0 .'
              }
       }
   }
}