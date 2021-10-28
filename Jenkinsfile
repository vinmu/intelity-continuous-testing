pipeline {
  agent any
  stages {
    stage('create reservation and check-in') {
      parallel {
        stage('create reservation and check-in') {
          steps {
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: '3BiaErzSpkm6jizPXF78Xg', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 600)
          }
        }

        stage('create reservation with cc/id checks enabled') {
          steps {
            sleep 19
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: 'NHuaKf242U6iD9CJliD13A', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 600)
          }
        }

      }
    }

    stage('place engineering dining requests and do cc id verification') {
      parallel {
        stage('place engineering dining requests and do cc id verification') {
          steps {
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: '_lX9tthpdEqsXdnYR-QO5Q', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 1200)
          }
        }

        stage('upsell category (tablet)') {
          steps {
            tpJobRun(projectId: 'eoeVUCkSFkucjcet2iJAKA', jobId: 'GBsqWGXGLkW49wx1HSdsuQ', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 1200)
          }
        }

        stage('place engineering request (iOS)') {
          steps {
            tpJobRun(projectId: 'eoeVUCkSFkucjcet2iJAKA', jobId: 'V4y7kbNL4ESgQOnsRpvgbA', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 1200)
          }
        }

      }
    }

    stage('check out reservation') {
      parallel {
        stage('check out reservation') {
          steps {
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', agentId: 'aJrwKYXc50ebvFZdq5w_1g', jobId: '8N730FcupEas_ngeMmy_BA', waitJobFinishSeconds: 600)
          }
        }

        stage('check out reservation and edit affiliate') {
          steps {
            sleep 17
            tpJobRun(projectId: 'o9PMCHqfb02X1hDACOa5hg', jobId: 'L3qgH0A0s0iNMOmCgNFWkQ', agentId: 'aJrwKYXc50ebvFZdq5w_1g', waitJobFinishSeconds: 600)
          }
        }

      }
    }

  }
}