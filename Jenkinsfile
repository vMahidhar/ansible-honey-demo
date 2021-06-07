pipeline{
    agent any
    stages{

        stage("installing apache"){
            steps{
                ansiblePlaybook become: true, credentialsId: 'AWS-SSH-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.inv', playbook: 'apache.yml'
            }
        }
    }
}