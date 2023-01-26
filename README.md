# visitCount

## Create AWS Lambda Python Function

For creating AWS Lambda function, I logged in AWS Console  
Search Lambda in bar

Create function--> name visitCountFunction--> select my Runtime which is going to be **Python 3.9 version**

Create Function--> Once function is been created, let's just go test it out.  

When you click test--> it shows new page where you need to create test event--> I'm gonna calling test event simple **hello**.

I can use the template, save that.  

When you click test, I can see that function executes, and here is response status code 200

Let's make test event have a user, because we wanna say hi to the user and delete other two keys.

And object I just configured, will be accessible in that event. Object passed to function

If I want to access user I called user = event["event"] and then access to key.

I'm gonna change to json message to  **'message': f"Hello {user}"**.

Click deploy and test it again, after test I can see Hello aruu_aws(username).

I create function which I can share with you in my github account

For now I have to accumulate times of visit of customers, so to do that I have figure out another way, Amazon Lambda is serverless service and I want to use Dynamo DB for this purpose.

I'll use AWS DynamoDB as a database for us to store information used by our Lambda functions.
