pipeline {
  agent any
  options {
    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
  }
  stages {
    stage ('Hello') {
      steps {
        echo "Hello"
      }
    }
  }
  // post {
  //   always {
  //       junit(
  //         allowEmptyResults: true, 
  //         testResults: '**/build/test-results/test/*.xml'
  //       )
  //   }
  // }
}





// pipeline {
//   agent {label 'linux'}
//   options {
//     buildDiscarder(logRotator(numToKeepStr: '5'))
//   }
//   stages {
//     stage('Build') {
//       steps {
//         sh './gradlew clean check --no-daemon'
//       }
//     }
//   }
//   post {
//     always {
//         junit(
//           allowEmptyResults: true, 
//           testResults: '**/build/test-results/test/*.xml'
//         )
//     }
//   }
// }