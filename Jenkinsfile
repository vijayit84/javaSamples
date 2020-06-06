pipeline
{
agent any
   environment
   {
   BRANCH_NAME:'master'
   }
stages
{
   stage("Build")
   {
    steps
    {
       
    echo "Build Step"
       echo "Branch Name : ${BRANCH_NAME}"   
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

}
