properties([pipelineTriggers([githubPush()])])

node {  

    git credentialsId: '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',
        url: scm.userRemoteConfigs[0].url, branch: 'main'
    
    stage('clone') { 
        echo 'cloning repo 1'
        echo 'cloning repo 2'
        sh '/working-files/build-scripts/do-clone.sh'        
    }
    stage('build') { 
      echo 'Output from stage 2'
      sh '/home/nms-adithyan/all-files/coding/repo/techsukras/groovy-training/groovy-training/src/training/day06/tupleconstr.groovy'
    }
    stage('Deploy') { 
        echo "Deployment Successful"
    }
}
