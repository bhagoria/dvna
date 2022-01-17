pipeline {
agent any
stages {
stage ('Source Composition Analysis') {
steps {
dependencyCheck additionalArguments: '''--project log4j
--scan */master
--format	HTML''', odcInstallation: 'OWASP'
}
}
}
}
