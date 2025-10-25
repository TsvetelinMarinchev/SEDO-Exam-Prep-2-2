pipeline{
    agent any
    stages{
        stage("Restore .NET packages"){
            steps{
               bat 'dotnet restore'
            }
        }
        stage("Build .NET Project"){
            steps{
               bat 'dotnet build --no-restore'
            }
        }
        stage("Run unit and integration Test"){
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
} 