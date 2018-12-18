node{
    stage('SCM Checkout'){
        git 'https://github.com/ramudevops123/mvn_bkp.git'
    }
    stage('Compile-Clean'){
        //Get maven homepath
        def M2_HOME = tool name: 'M2_HOME', type: 'maven'
        sh "${M2_HOME}/bin/mvn clean"
    }
    stage('Compile-Package'){
        //Get maven homepath
        def M2_HOME = tool name: 'M2_HOME', type: 'maven'
        sh "${M2_HOME}/bin/mvn package"
    }
    stage('Compile-Install'){
        //Get maven homepath
        def M2_HOME = tool name: 'M2_HOME', type: 'maven'
        sh "${M2_HOME}/bin/mvn install"
    }
    stage('Compile-Deploy'){
        //Get maven homepath
        def M2_HOME = tool name: 'M2_HOME', type: 'maven'
        sh "${M2_HOME}/bin/mvn deploy"
    }
}
