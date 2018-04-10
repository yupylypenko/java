pipeline {
    agent any
    stages{
      stage ('Compile Stage') {
        steps{
          withMaven (maven : 'maven_3_5_3') {
            sh 'mvn compile'
          }
        }

      }
      stage ('Testing Stage') {
        steps{
            sh 'echo Test'
        }

      }
      stage ('Deployment Stage') {
        steps{
          sh 'echo Deploy'
          }

      }
    }
}
