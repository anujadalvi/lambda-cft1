pipeline{
	agent any
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name ${stackname} --template-body file://lambda_cft.json --parameters ParameterKey='function_name',ParameterValue='${func_name}' --region 'us-east-1'"
			}
	}
		
	
	}
}
