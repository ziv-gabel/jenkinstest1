def myPipeline
node('dev') {
    checkout([
        $class: 'GitSCM',
        branches: scm.branches,
        doGenerateSubmoduleConfigurations: true,
        extensions: scm.extensions + [[$class: 'SubmoduleOption', parentCredentials: true]],
        userRemoteConfigs: scm.userRemoteConfigs
    ])
    myPipeline = load "jenkinstest2/Jenkinsfile"
}

