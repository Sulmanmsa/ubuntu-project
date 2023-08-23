pipeline{
    agent any
    tools{
        maven 'Maven'
    }
    stages{
        stage("Test"){
            steps{
                sh "mvn test"
            }
           
        }
        stage("build"){
            steps{
                sh 'mvn clean package'
            }
        }
        stage("deploy"){
            steps{

            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
