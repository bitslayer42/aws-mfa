# aws-mfa
Python script to use AWS Two Factor Authentication on the Command Line

To set up, enter the name of your MFA Device in mfa_config.py

To use:

- Look up a 6 digit code on your device.

- Run script: 
```
    python mfa.py
```
- Enter code when prompted.
The commands you need will be printed out below.
They will look something like this:
```
    export AWS_ACCESS_KEY_ID="ASI..."
    export AWS_SECRET_ACCESS_KEY="CZb..."
    export AWS_SESSION_TOKEN="IQoJc..."
```
- Copy and paste to command line.

To verify, a simple command that should work might be:
```
    aws s3 ls
```
