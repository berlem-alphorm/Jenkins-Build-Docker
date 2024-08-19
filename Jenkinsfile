
nade{
  def app
  
    stage('clone'){
        checkout scm
}
stage('Build image') {
    app = docker.build("berlem/nginx")
}

stage('Run image'){
    docker.image('berlem/nginx').withRun('-p 80:80') {c -> 
    sh 'docker ps'
    sh 'curl locathost'

   }
 }
}
