# GPR
Use this script to create Bitbucket pull requests from the command line

## Installing
Download the script, move it to */usr/local/bin/gpr* and make sure you have access to execute it:
```
mv gpr /usr/local/bin/gpr
chmod +x /usr/local/bin/gpr
```

## Configuration
You will need to create a BitBucket Personal Access Token, click [here](https://confluence.atlassian.com/bitbucketserver/personal-access-tokens-939515499.html) for more information.
Then, specify the Bitbucket domain. Both should be passed as environment variables. You can use the */etc/profile* file to store these variables.
```
export GPR_BITBUCKET_PERSONAL_ACCESS_TOKEN=AzU5NEMyMTcyODM1YpArpyl7v2IghlBUMtjbrZKvI/xK
export GPR_GIT_DOMAIN=git.company.com
```

## Usage
Execute the script passing the title of the PR as a parameter:
```
gpr "Updating libraries"
```
