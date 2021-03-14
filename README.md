# Marval EC2 Creator

<p>This cloudformation template allows you to create an API protected endpoint to create new EC2 servers.
This is primarily designed for Marval however it can work with anything that can run a webhook with headers.
Simply click on 'Launch Stack' in whatever region you like and you will be taken to the cloudformation page to launch your stack.
The output will provide you with two pieces of information to run your API.</p>
<ul>
<li>RESTFul Endpoint from API Gateway</li>
<li>API Key</li>
</ul>
<h2>RESTFul Endpoint</h2>

<h2>API Key</h2>

![Hello World](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEYAAAAUCAAAAAAVAxSkAAABrUlEQVQ4y+3TPUvDQBgH8OdDOGa+oUMgk2MpdHIIgpSUiqC0OKirgxYX8QVFRQRpBRF8KShqLbgIYkUEteCgFVuqUEVxEIkvJFhae3m8S2KbSkcFBw9yHP88+eXucgH8kQZ/jSm4VDaIy9RKCpKac9NKgU4uEJNwhHhK3qvPBVO8rxRWmFXPF+NSM1KVMbwriAMwhDgVcrxeMZm85GR0PhvGJAAmyozJsbsxgNEir4iEjIK0SYqGd8sOR3rJAGN2BCEkOxhxMhpd8Mk0CXtZacxi1hr20mI/rzgnxayoidevcGuHXTC/q6QuYSMt1jC+gBIiMg12v2vb5NlklChiWnhmFZpwvxDGzuUzV8kOg+N8UUvNBp64vy9q3UN7gDXhwWLY2nMC3zRDibfsY7wjEkY79CdMZhrxSqqzxf4ZRPXwzWJirMicDa5KwiPeARygHXKNMQHEy3rMopDR20XNZGbJzUtrwDC/KshlLDWyqdmhxZzCsdYmf2fWZPoxCEDyfIvdtNQH0PRkH6Q51g8rFO3Qzxh2LbItcDCOpmuOsV7ntNaERe3v/lP/zO8yn4N+yNPrekmPAAAAAElFTkSuQmCC)


<!DOCTYPE html>
<html lang="en">
  <head>
   
  </head>
  <body>
    
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
