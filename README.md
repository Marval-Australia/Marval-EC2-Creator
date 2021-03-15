# Marval EC2 Creator


<!DOCTYPE html>
<html lang="en">
  <head>
   
  </head>
  <body>

<p>This cloudformation template allows you to create an API protected endpoint to create new EC2 servers.
This is primarily designed for Marval however it can work with anything that can run a webhook with headers.
Simply click on 'Launch Stack' in whatever region you like and you will be taken to the cloudformation page to launch your stack.
The output will provide you with two pieces of information to run your API.</p>
<ul>
<li>RESTFul Endpoint from API Gateway</li>
<li>API Key</li>
</ul>
<h2>Setting up your AWS EC2 Integration</h2>

<h3>Step 1 - Create an Action Message</h3>
<p>The restful endpoint is placed into Marval under the webhook information. The first step is to create an Action Message which will contain the information which is POSTed to the webhook. To create an action message, navigate to <b>Maintenance | Request | Action Messages</b>. The following is an example of an Action Message which is used to create an instance with Template ID lt-0037fr5582b0da15e.</p>

```javascript
{
   "TemplateID": "lt-0037fr5582b0da15e",
   "NotificationEmailAddress": "@Model.PreferredNotification.Address",
   "RequestNumber": "@Model.RequestNumber",
   @foreach (var item in Model.Attributes){	
      @:"@item.Type.Name": "@item.Value",
   }
   "NotificationFromAddress": "YourEmailAddress"
}
```
<h3>Step 1 - Create an Request Action</h3>
<p>Once this action message is created, navigate to <b>Maintenance | Request | Request Actions</b> and create a new request action with 'When' criteria. Under 'Then' criteria, select 'Webhook to URL', then paste in your URL from the output of your Cloudformation Stack. the Verb to use is 'Post' and the Body is the Action Message you created in the previous step. Add a key value pair as a Header, under the 'including Headers' section. The key is x-api-key and the Value is the API Key in the output of your cloudformation stack.</p>

<h2>API Key</h2>

<table>
<tr>
<th>Region</th>
<th>cfn.template</th>
</tr>
<tr>
<th>eu-north-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=eu-north-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-eu-north-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ap-south-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ap-south-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ap-south-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>eu-west-3</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=eu-west-3#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-eu-west-3/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>eu-west-2</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=eu-west-2#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-eu-west-2/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>eu-west-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=eu-west-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-eu-west-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ap-northeast-3</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ap-northeast-3#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ap-northeast-3/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ap-northeast-2</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ap-northeast-2#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ap-northeast-2/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ap-northeast-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ap-northeast-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ap-northeast-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>sa-east-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=sa-east-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-sa-east-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ca-central-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ca-central-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ca-central-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ap-southeast-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ap-southeast-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>ap-southeast-2</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-2#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-ap-southeast-2/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>eu-central-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=eu-central-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-eu-central-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>us-east-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-us-east-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>us-east-2</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-us-east-2/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>us-west-1</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=us-west-1#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-us-west-1/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
<tr>
<th>us-west-2</th>
<td>
<a href="https://console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/new?stackName=Marval-EC2-Creator-cfn&templateURL=https://s3.amazonaws.com/cfn-742226607901-us-west-2/Marval-EC2-Creator/latest/cfn.template">
<img alt="Launch Stack" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png" />
</a>
</td>
</tr>
</table>
<p class="footer">Generated by cfn-publish on Wed Mar 10 00:55:03 UTC 2021</p>
</body>
</html>

