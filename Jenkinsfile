pipeline{
    agent any
    stages{
        stage("Restore dependencies"){
            steps{
                bat 'dotnet restore'
            }
        }
        stage("Build"){
            steps{
                bat 'dotnet restore'
            }
        }
        stage("Run Project1 Tests"){
            steps{
                bat 'dotnet test TestProject1 --nobuild --verbosity normal'
            }
        }
        stage("Run Project2 Tests"){
            steps{
                bat 'dotnet test TestProject2 --nobuild --verbosity normal'
            }
        }
        stage("Run Project3 Tests"){
            steps{
                bat 'dotnet test TestProject3 --nobuild --verbosity normal'
            }
        }
    }
}