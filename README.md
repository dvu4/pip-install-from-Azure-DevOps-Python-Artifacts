#   Install a package from our Azure DevOps Artifacts feed 

Package from our Azure DevOps Artifacts is internal package, we can not download directly. 


If we want to install `dai-identity-api` package

![python-package](./docs/image1.png)

`pip install dai-identity-api` will not work. We will need to pass extra index url

- Step 1 : Create 

![Scenario2](./docs/image2.png)

![Scenari3](./docs/image4.png)

![Scenario4](./docs/image5.png)

![Scenario5](./docs/image6.png)

- Step 2 : 
`pip install <python-package>   --extra-index-url https://pkgs.dev.azure.com/<your-organization-name>/<your-project-name>/_packaging/<your-feed-name>/pypi/simple

in this case : `pip install dai-python-logging --extra-index-url https://pkgs.dev.azure.com/WBA/DAI/_packaging/DAI/pypi/simple`

- Step 3 :
