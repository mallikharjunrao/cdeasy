node {
  stage 'Deploy to Integration'
    checkout scm
    gitCommit = sh(returnStdout: true, script: 'git rev-parse HEAD').trim()
    shortCommit = sh(returnStdout: true, script: 'git rev-parse HEAD').trim().take(6)
    echo "Here goes the unit level tests ${shortCommit}"
    sh 'printenv'
    echo 'Here goes the code linting'
    sh 'sleep 5s'
}
