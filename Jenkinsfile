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
stage ('publishreport') 
{
steps 
{ dependencyCheckPublisher pattern: '**/dependency-check-report.xml'}
}
}
}
