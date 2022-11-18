pipeline{
    agent any
    stages{
        stage('git_clone'){
            steps{
                sh'''
                pwd
                rm -rf *
                git clone "https://github.com/haseenashaikh/repractice.git"
                '''
            }
        }
        stage('maven'){
            steps{
                sh'''
                cd repractice
                mvn clean
                '''
            }
        }
        stage('maven-1'){
            steps{
                sh'''
                cd repractice
                mvn test
                '''
            }
        }
        stage('maven-2'){
            steps{
                sh'''
                cd repractice
                mvn compile
                '''
            }
        }
    }
}
