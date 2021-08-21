def workspace
node
{
    stage('Checkout')
    {
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: '1c9cef13-5586-4c1d-bbc4-8b0113a07f81', url: 'https://github.com/sahi1999/FirstRepo.git']]]) 
        workspace =pwd()
    }
    stage('Static Code Analysis')
    {
        echo 'Static Code Analysis'
    }
    stage('Build')
    {
        echo 'Build the code'
    }
    stage('Unit Testing')
    {
        echo 'Unit Testing'
    }
    
}
