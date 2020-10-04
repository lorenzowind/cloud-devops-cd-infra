1. aws cloudformation deploy \
  --template-file infra.yml \
  --stack-name production-distro \
  --parameter-overrides PipelineID="${S3_BUCKET_NAME}" \
  --tags project= &