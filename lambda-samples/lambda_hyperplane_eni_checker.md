## Lambda Hyperplane ENI checker

[This function](lambda-samples/llambda_hyperplane_eni_checker.py) checks against Lambda function(s) and its layers if they are using a particular ENI. If you come across ``` You are not allowed to manage 'ela-attach' attachments ``` error while trying to manually delete the ENI, this might be useful.

Provide the input parameters:

```python
...
region = 'us-west-2'
eni_name = 'eni-XXXXXXXXXXXXXXXXX'
...

```


Output:

```

Lambda function(s) using ENI: eni-XXXXXXXXXXXXXXXXX:

arn:aws:lambda:us-west-2:XXXXXXXXXXXX:function:LambdaconnectingtoLambda2:$LATEST
arn:aws:lambda:us-west-2:XXXXXXXXXXXX:function:ThisFunctionDoesNothing:$LATEST


```