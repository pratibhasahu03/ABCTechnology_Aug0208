pipeline
{
    agent any
    stages
    {
        stage('Code Checkout')
        {
            steps
            {
                git 'https://github.com/pratibhasahu03/ABCTechnology_Aug0208.git'
            }
        }
        stage('Code Compile')
        {
            steps
            {
                sh 'mvn compile'
            }
        }
        stage('Code Test')
        {
            steps
            {
                sh 'mvn test'
            }
        }
        stage('Code Package')
        {
            steps
            {
                sh 'mvn package'
            }
        }
    }
}
