def myPipeline
node {
    checkout scm // mandatory
    myPipeline = load "jenkinstest2/Jenkinsfile"
}
myPipeline()
