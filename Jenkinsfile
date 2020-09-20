/* pipeline {
    agent any

        environment {
            URL1 = 'google.com'
        }

        triggers { pollSCM('H/2 * * * *') }

        parameters {
                string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

                text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

                booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

                choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

                password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
            }

        tools {
            terraform 'terraform-0.12.29'

        }

    stages {

        stage ('My First Stage') {
            environment {
                        URL2 = 'yahoo.com'
                    }
            steps {
                sh '''
                  echo Hello from First Stage
                  ls
                  echo Bye from First Stage
                '''
                print "Hello Groovy"
                print "URL1 = " + URL1
                print "URL2 = " + URL2
            }
        }

        stage('Conditional Stage') {
            when {
                expression {
                    return params.TOGGLE
                }
            }


            steps {
                print 'Conditional Stage'
            }
        }


        stage ('My Second Stage') {
            steps {
             print 'Second Stage'
             input message: 'Should we continue?', ok: 'Yes we should.', parameters: [password(defaultValue: '', description: '', name: 'PIN')], submitter: 'admin'

            }

        }

        stage ('Terraform Version') {
            steps {
            sh 'terraform version'
            }
        }
    }
}
*/

/*
pipeline {
    agent none
    stages {
        stage('Non-Sequential Stage') {
            agent any
            steps {
                echo "On Non-Sequential Stage"
            }
        }
        stage('Sequential') {
            agent any
            environment {
                FOR_SEQUENTIAL = "some-value"
            }
            stages {
                stage('In Sequential 1') {
                    steps {
                        echo "In Sequential 1"
                    }
                }
                stage('In Sequential 2') {
                    steps {
                        echo "In Sequential 2"
                    }
                }
                stage('Parallel In Sequential') {
                    parallel {
                        stage('In Parallel 1') {
                            steps {
                                echo "In Parallel 1"
                            }
                        }
                        stage('In Parallel 2') {
                            steps {
                                echo "In Parallel 2"
                            }
                        }
                    }
                }
            }
        }
    }
}
*/

@Library('roboshop') _
sample.info 'Starting'
sample.warning 'Nothing to do!'

/*
pipeline {
    agent any

    stages {
        stage('Sample') {
         steps {
            script {
                sample()
            }
         }
        }
        }
    }
    */
