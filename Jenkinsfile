node
{
  def remote = [:]
    remote.name = 'Devesh'
    remote.host = '192.168.1.8'
    remote.user = 'root'
    remote.password = 'toor'
    remote.allowAnyHosts = true
    stage('Remote SSH') {
      sshCommand remote: remote, command: "ls -lrt"
    //  sshCommand remote: remote, command: "for i in {1..5}; do echo -n \"Loop \$i \"; date ; sleep 1; done"
    }
    stage('Install Localy file')
  {
    sh 'apt-get install $program'
  }
  
}
