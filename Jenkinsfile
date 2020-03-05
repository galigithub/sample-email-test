node {
    stage('git'){
        git 'https://github.com/allure-examples/allure-testng-example.git'
    }
    
    stage('actions'){
        emailext body: '''${SCRIPT, template="build-report.groovy"}''',
                subject: "[Jenkins] REPORT",
                to: "shivakumargali83@gmail.com"
    }
}
