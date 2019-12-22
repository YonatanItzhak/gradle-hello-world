node('slave1') {
  def grdlHome = tool 'gradle4'
    try {
  stage('Checkout'){
    checkout scm
  }
  stage('Build'){
    sh "${grdlHome}/bin/gradle build"
  }
//  stage('Unit-test'){
//    sh "${grdlHome}/bin/gradle test"
//    junit '**/build/test-results/*/*.xml'
//  }
//  stage('Func-test'){
//    tests = ["one" : { sh "test-data/int-test.sh build/libs/oto-gradle-1.0.jar OtoMato 'Hello Otomato!'"},
//         "two" :{ sh "test-data/int-test.sh build/libs/oto-gradle-1.0.jar YoNatAn 'Hello Yonatan!'" },
//                 "three" :{ sh "test-data/int-test.sh build/libs/oto-gradle-1.0.jar WoRlD 'Hello World!'" }]
//     
//  }
// parallel tests
    }
  catch(ex) {echo 'there were failures'  }
  stage(‘Post’) {
    echo 'I will always love you!'  
  }
}
