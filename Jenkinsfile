pipeline
{
    agent none
    stages
    {
        stage('Code Checkout and compile')
        {
            agent {label ‘Slave1’}
            steps
            {
                git branch:'main', url:'https://github.com/pratibhasahu03/ABCTechnology_Aug0208.git'
                sh 'mvn compile'
            }
        }
        stage('Code Test')
        {
	        agent {label ‘Slave2’ }
            steps
            {
                sh 'mvn test'
            }
        }
        stage('Code Package')
        {
	        agent {label ‘Slave3’ }
            steps
            {
                sh 'mvn package'
            }
        }
    }
}
