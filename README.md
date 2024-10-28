# wheel-job-sample
This repo is a demo on how you can create a wheel from Python, then add it as a job to Databricks workflows.

## Instructions
Follow this: https://docs.databricks.com/en/jobs/how-to/use-python-wheels-in-workflows.html

The repo already contains the required folder structure. You can build on this. 

To create the wheel, run:

```python3 setup.py bdist_wheel```

Then you can create a task, specify `run` as the entry point, add the wheel as a dependency, and run the task! Task parameters will ba passed onto the code in `sys.argv`. 