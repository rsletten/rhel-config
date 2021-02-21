pipeline {
    agent {label 'master'}
    options {
        ansiColor('xterm')
    }
    stages {
        stage("RHEL Configure") {
        steps {
            sh "export ANSIBLE_HOST_KEY_CHECKING=False && ANSIBLE_FORCE_COLOR=true && ansible-playbook -i inventory rhel-configure.yaml"
        }
    }
  }
}
