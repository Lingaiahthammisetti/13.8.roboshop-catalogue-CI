@Library('jenkins-shared-library-for-roboshop')

// create variable of map type and set the values
def configMap = [
    //type: "nodejsEKS",
    component: "catalogue",
    project: "roboshop"
]
echo "test:"
if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
      nodeJSEKSPipeline(configMap)
    //pipelineDecision.decidePipeline(configMap)
}
else{
    echo "Proceed with CR or NON-PROD pipeline"
}