pipeline {
    agent any
    stages{
      stage ('Compile Stage') {
        steps{
          withMaven (maven : 'maven_3_5_3') {
            sh 'echo Compile'
          }
        }

      }
      stage ('Testing Stage') {
        steps{
          withMaven (maven : 'maven_3_5_3') {
            sh 'echo Test'
          }
        }

      }
      stage ('Deployment Stage') {
        steps{
          withMaven (maven : 'maven_3_5_3') {
            sh 'echo Deploy'
          }
        }

      }
    }
}
