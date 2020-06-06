pipeline
{
agent any
       parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?'),
        choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: 'select Choices')        
       
       }

   environment
   {
   BRANCH_NAME='master'
   }
stages
{
   stage("Build")
   {
    steps
    {
       
    echo "Build Step"
       echo "Branch Name : ${BRANCH_NAME}"   
       echo "Parameter :${params.Greeting}"
    }
   
   }
stage("Test")
   {
    steps
    {
    echo "Test Step"
    }
   
   }
stage("Deploy")
   {
    steps
    {
    echo "Deploy Step"
    }
   
   }

}
       post {
        success
       {
        echo "Success Job"
       }
    }

}
