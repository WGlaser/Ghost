pipeline {
         agent any
         stages {
                 stage('Build') {
                 steps {
                     echo 'Hi, Wade. Building App'
                 }
                 }
                 stage('Test') {
                 steps {
                    input('Do you want to proceed?')
                 }
                 }
               
                 stage('Prod') {
                     steps {
                                echo "App is Prod Ready"
                              }
                 
              }
}
}
