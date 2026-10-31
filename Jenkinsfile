// we need to refer pipeline from centralised library
// we have created shared library pipelines in jenkins-shared-library repo and added it under jesnkins system global trusted pipeline libraries

@Library('Jenkins-shared-library')_ //name proivded in jenkins global trusted pipeline libraries

def configMap=[
    project: "roboshop",
    component: "shipping"
]

if (! env.BRANCH_NAME.equalsIgnoreCase('main')){
    JavaEKSPipeline(configMap)
}
else{
    echo "please follow CR process"
}