node{

    stage("Git Clone"){
        git credentialsId: '3c57c31d-7e69-4389-828b-f27eab7cb945', url: 'https://github.com/AnkitVarshney081/CI-CD-Pipeline.git'
    }

    stage("Maven Clean Build"){
        
        def mavenHome = tool name: "maven3" , type: "maven"
        def mavenCMD = "${mavenHome}/bin/mvn "
        sh "${mavenCMD} clean package"
    }
}

