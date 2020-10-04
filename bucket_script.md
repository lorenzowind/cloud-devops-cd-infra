1. aws cloudformation deploy \
  --template-file bucket.yml \
  --stack-name "${CIRCLE_WORKFLOW_ID:0:7}" \
  --parameter-overrides PipelineID="${CIRCLE_WORKFLOW_ID:0:7}"