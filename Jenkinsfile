pipeline 
{
agent any
stages 
{
stage ('Source Composition Analysis') 
{
steps 
{
dependencyCheck additionalArguments: '''--project log4jPipeline
--format	HTML''', odcInstallation: 'OWASP'
}
}
}
}
