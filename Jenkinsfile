pipeline{
agent any
stages
{
stage("Code Checkout")
{
steps
{
echo "Testing Code checkout"
}
}
stage("Code compilation")
{
steps
{
sh "javac WebhooksExampleNew.java"
}
}
stage("Code Execution")
{
steps
{
sh "java WebhooksExampleNew"
}
}
stage("App Health Check")
{
steps
{
sh "curl http://ip172-18-0-6-c5cu0bnnjsv0009vm07g-9090.direct.labs.play-with-docker.com/"
}
}
stage("Publish Report")
{
steps
{
echo "Sending Emails"
}
}
}
}
