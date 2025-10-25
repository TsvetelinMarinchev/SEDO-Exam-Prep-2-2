pipeline{
    agent any
    stages{
        stage("Build .NET Project"){
            steps{
               bat 'dotnet build'
            }
        }
        stage("Run unit and integration Test"){
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
} 