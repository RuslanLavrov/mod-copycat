buildMvn {
  publishModDescriptor = true
  mvnDeploy = true
  publishAPI = true
  runLintRamlCop = true
  buildNode =  'jenkins-agent-java11'

  doDocker = {
    buildJavaDocker {
      publishMaster = true
      healthChk = true
      healthChkCmd = 'curl -sS --fail -o /dev/null  http://localhost:8081/apidocs/ || exit 1'
    }
  }
}

