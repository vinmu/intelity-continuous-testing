pipeline {
  agent any
  stages {
    stage('create reservation and check-in') {
      parallel {
        stage('create reservation and check-in') {
          steps {
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: '3BiaErzSpkm6jizPXF78Xg', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 360)
          }
        }

        stage('create reservation with cc/id checks enabled') {
          steps {
            sleep 21
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: 'NHuaKf242U6iD9CJliD13A', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 360)
          }
        }

      }
    }

    stage('place engineering dining requests and do cc id verification') {
      steps {
        tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: '_lX9tthpdEqsXdnYR-QO5Q', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 1200)
      }
    }

  }
}