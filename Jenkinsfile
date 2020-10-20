//@Library("github.com/Jim-Dawson-EMR/libraryTest@${ENV:ENVIRONMENT}") _
//library identifier: '', retriever: modernSCM(github(traits: [gitHubBranchDiscovery(1), gitHubPullRequestDiscovery(1), gitHubForkDiscovery(strategyId: 1, trust: gitHubTrustPermissions())], credentialsId: 'ad3fcc3e-3a27-4c7e-b5b1-1b5fd8f9eca9', repository: 'libraryTest', repoOwner: 'Jim-Dawson-EMR'))
library("github.com/Jim-Dawson-EMR/libraryTest@${ENV:ENVIRONMENT}")

pipeline {
    agent any

    stages {
        stage('show branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage("libary function no arg") {
            steps {
                script {
                    helloWorld()
                }
            }            
        }
        stage("libary function with arg") {
            steps {
                script {
                    helloArgs('Jenkins!')
                }
            }            
        }
        stage("addl libary function with arg") {
            steps {
                script {
                    helloArgs.goodbyeWorld('Jenkins!')
                }
            }            
        }
    }
}
