# visitCount
## Create AWS Lambda Python Function
For creating AWS Lambda function, I logged in AWS Console  
Search Lambda in bar  
Create function--> name visitCountFunction--> select my Runtime which is goung to be **Python 3.9 version**   
Create Function--> Once fucntion is been created, let's just go test it out.  
When you click test--> it shows new page where you need to create test event-->   
I'm gonna calling test event simple **hello**. 
I can use the template, save that.  
When you click test, I can see that function executes, anh here is response status code 200   
Let's make test event have a user, because we wanna say hi to the user and delete other two keys. 
And object I just configured, will be accessible in that event. Object passed to function   
If I want to access user I called user = event["event"] and then access to key. 
I'm gonna change to json message to  **'message': f"Hello {user}"**. 
Click deploye and test it again, after test I can see Hello aruu_aws(username). 

