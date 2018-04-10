pipeline {
    agent any
    stages{
      stage ('Compile Stage') {
        steps{
          withMaven (maven : 'Maven_3_5_3') {
            sh 'mvn compile'
          }
        }

      }
      stage ('Testing Stage') {
        steps{
          withMaven (maven : 'Maven_3_5_3') {
            sh 'mvn test'
          }
        }

      }
      stage ('Deploy Stage') {
        steps{
          withMaven (maven : 'Maven_3_5_3') {
            sh 'mvn package'
          }
        }

      }
    }
}
