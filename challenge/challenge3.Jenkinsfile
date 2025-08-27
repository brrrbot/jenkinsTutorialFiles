pipeline {
    agent any

    parameters {
        string(defaultValue: "", description: "What is the deployment name?", name: "deployName")
        choice(choices: ["EU-WEST-2A", "EU-WEST-2B", "EU-WEST-2C"], description: "What is the deployment AZ?", name: "deployRegion")
        booleanParam(defaultValue: false, description: "Confirm deployment?", name: "deployBoolean")
    }

    stages {
        stage("Demo") {
            steps {
                echo "name: ${params.deployName}"
                echo "Region: ${params.deployRegion}"
                echo "status: ${params.deployBoolean}"
            }
        }
    }
}