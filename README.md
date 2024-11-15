<h2> MLflow Demo </h2>

import dagshub
dagshub.init(repo_owner='DeepakMishra99', repo_name='mlflow_demo', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)