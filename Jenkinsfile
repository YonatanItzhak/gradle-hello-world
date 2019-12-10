node('slave') {
  def grdlHome = tool 'gradle4'
  stage('Checkout'){
    checkout scm
  }
  stage('Build'){
    sh "${grdlHome}/bin/gradle build"
  }
}
