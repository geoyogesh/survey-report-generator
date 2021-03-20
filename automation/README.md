Pre
https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-windows.html


aws cloudformation deploy --template-file survey-report-generator-persistance.yml  --stack-name survey-report-generator-persistance-dev --parameter-overrides BuildProjectName=survey-report-generator EnvironmentName=dev --capabilities=CAPABILITY_NAMED_IAM



aws cloudformation deploy --template-file survey-report-generator-ci-cd.yml  --stack-name survey-report-generator-ci-cd-common --parameter-overrides BuildProjectName=survey-report-generator EnvironmentName=common --capabilities=CAPABILITY_NAMED_IAM