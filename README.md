# Send-Mail-With-Go
Send an Email through AWS SES with GoLang - AWS SDK

## Verify your email address
* Open the AWS SES Console.
* Choose Verified identities under Configuration
* Click create identity
* On the opened window, select Email address as a identity type.
* Type your email address
* Click Create identity
* To verify email address, check your email box, there will be an email from Amazon Web Services about Email Address Verification Request.


## Install the AWS SDK for Go

```bash
go get -u github.com/aws/aws-SDK-go/...
```

## Get your AWS Access Keys

* Open the IAM console.
* On the navigation menu, choose Users.
* Choose your IAM user name (not the check box).
* Open the Security credentials tab, and then choose to Create access key.
* To see the new access key, choose Show. Your credentials resemble the following: Access key ID: AKIAIOSFODNN7EXAMPLE Secret access key: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
* To download the key pair, choose the Download .csv file. Store the keys in a secure location.

## Config Setup

* Your AWS config and credentials will be stored under ~/.aws/config and ~/.aws/credentials. Those are the default values for your AWS SDK Environment. If you want you can edit them.

* Run the below command in the terminal to let the Go Program know that it should pick up the AWS config from the ~/.aws directory

```bash
export AWS_SDK_LOAD_CONFIG=true
```


## Execution

```bash
go run main.go
```

After run the code, You will see such an output:

Email sent to address:alizkl.cs@gmail.com
{
MessageId: "01000183092d8266-239d2851-2838-4b50-af01-9af759710c7e-000000"
}
