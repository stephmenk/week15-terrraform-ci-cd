pipeline{
    agent any
    stages{
        stage(ibit){
            steps{
                sh 'terraform init'
            }
        }
        stage(format){
            steps{
                sh 'terraform fmt'
            }
        }
        stage(validate){
            steps{
                sh 'terraform validate'
            }
        }
        stage(plan){
            steps{
                sh 'terraform plan'
            }
        }
        stage(apply){
            steps{
                sh 'terrform apply --auto-approve'
            }
        }
        stage(destroy){
            steps{
                sh 'terraform destroy --auto-approve'
            }
        }
    }
}