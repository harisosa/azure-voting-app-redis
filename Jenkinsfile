pipeline {
   agent any

   stages {
      stage('Verify Branch') {
         steps {
            env.GIT_COMMIT = sh(script: "git rev-parse HEAD", returnStdout: true).trim()
            echo env.GIT_COMMIT
            echo "$GIT_BRANCH"
         }
      }
   }
}

