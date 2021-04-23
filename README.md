Project Overview
- Run Project locally
- In order to get both Docker and WSL2 to work correctly I had to enable my VM within my BIOS settings.
- To build the container I had to create a dockerfile with my corresponding image which stands up an Apache2 server with my small html file used as the page.
- to run the container you used the docker build to create the image and then docker run with my specified items.
- to view the project I simply type my ip/80 into the bar for entering websites within chrome.

- Configure AWS CLI
- IAM credentials were given through class
- had difficulty installing this because I was trying to get the wrong version.
- had to curl a zip file from AWS, unzip the file, and then install AWS with what was within the zip
- Once installed, you AWS configure, with the credentials given for class.

- Create ECR
- aws ecr create-repository --repository-name /w015ajo  --region us-east-1

- Configure Github Secrets
- With our credentials freom class we go into our created github repository and set the secrets within the secrets tab. These are both the credentials and the secret key.

- Configure Github Workflow
- Within the work flow you need to change the region and image name in order for the docker to build the image correctly.
