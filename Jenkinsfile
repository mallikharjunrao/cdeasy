node {
  stage 'Deploy to Integration'
    checkout scm
    gitCommit = sh(returnStdout: true, script: 'git rev-parse HEAD').trim()
    shortCommit = sh(returnStdout: true, script: 'git rev-parse HEAD').trim().take(8)
    SHORT=sh(returnStdout: true, script: 'git rev-parse HEAD').trim().take(8)
    withEnv(["GIT_COMMIT=${shortCommit}"]) {
      echo "Here is the commit ${GIT_COMMIT}"
      sh 'printenv'
    }
    sh 'printenv'
}
