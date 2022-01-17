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
--scan */master
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
