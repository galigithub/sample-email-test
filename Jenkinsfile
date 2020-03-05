node {
    stage('git'){
        git 'https://github.com/allure-examples/allure-testng-example.git'
    }
    
    stage('email'){
        emailext body: '''${SCRIPT, template="groovy-html.template"}''',
            mimeType: 'text/html',
            subject: "[Jenkins] REPORT",
            to: "shivakumargali83@gmail.com"
    }
}
