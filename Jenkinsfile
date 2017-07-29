node {
  stage('save') {
    checkout scm
    archiveArtifacts 'README.md'
  }
}

build job: 'playground/configure', parameters: [[$class: 'StringParameterValue', name: 'BRANCH_NAME', value: env.BRANCH_NAME]], quietPeriod: 2, wait: false
