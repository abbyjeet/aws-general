# General AWS stuff

## Installing AWS CLI
```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && \
unzip awscliv2.zip && \
sudo ./aws/install
```

## Uninstall AWS CLI
```
sudo rm -rf /usr/local/aws-cli | sudo rm /usr/local/bin/aws*
```

## Configure AWS CLI
1. Click on user menu
2. Security Credentials
3. In AWS IAM Credentials tab, click on Create access key
4. This will generate Access Key ID and Secret Access Key. Downlaod CSV and also copy/paste the Key Id and Secret to the prompts, as they will not be visible again
5. Region ID you can get from Region selector menu
6. Output format can be JSON, YAML, YAML stream, Text or Table

```
$aws configure
AWS Access Key ID [None]: AKIA47VCHBDRGXJB5CEH
AWS Secret Access Key [None]: 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
Default region name [None]: ap-southeast-2
Default output format [None]: json
```

You can now try the commands such as:
```
aws configure list-profiles
aws configure list
```


## Installing Boto3
First ensure that python3.6+ and pip are installed  
```
pip install boto3
```

## Uninstalling Boto3
```
pip uninstall boto3
```
