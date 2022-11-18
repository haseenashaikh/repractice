pipeline{
    agent any
    stages{
        stage('git_clone'){
            steps{
                sh'''
                pwd
                rm -rf *
                git clone ""
                '''
            }
        }
        stage('maven'){
            steps{
                sh'''
                pwd
                rm -rf *
                mvn clean
                '''
            }
        }
        stage('maven-1'){
            steps{
                sh'''
                pwd
                rm -rf *
                mvn test
                '''
            }
        }
        stage('maven-2'){
            steps{
                sh'''
                pwd
                rm -rf *
                mvncompile
                '''
            }
        }
    }
}
