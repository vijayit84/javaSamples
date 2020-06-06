pipeline
{
agent any
       parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
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
       
        failure {
            mail to: vijay.it84@gmail.com, subject: 'The Pipeline failed :('
        }
        success
       {
          mail to :vijay.it84@gmail.com, subject:'The Pipeline Success :)'
       }
    }

}
