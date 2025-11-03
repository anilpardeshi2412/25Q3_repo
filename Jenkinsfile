pipeline{
        agent{
              label{
                    label "built-in"
                            customWorkspace "/mnt/webhook1"
              }
        }
        stages {
                  stage ('satge-1'){
                          steps {
                                    sh '''
                                          rm -rf /var/www/html/index.html
                                          cp /mnt/webhook1/index.html /var/www/html/
                                          chmod 777 /var/www/html/index.html
                                          '''
                                            }
                  }
        }
}
