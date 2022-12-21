#   Install a package from our Azure DevOps Artifacts feed 

Package from our Azure DevOps Artifacts is internal package, we can not download directly. 


For example,  we want to install `dai-python-logging` package

![python-package](./docs/image1.png)

`pip install dai-identity-api` will not work. We will need to pass extra index url

- Step 1 : Create username and password

![Scenario2](./docs/image2.png)

![Scenario4](./docs/image4.png)


![Scenario5](./docs/image5.png)

Token is created
![Scenario3](./docs/image3.png)
- Step 2 : Install a Python package from Azure DevOps Artifacts
`pip install <python-package>   --extra-index-url https://pkgs.dev.azure.com/<your-organization-name>/<your-project-name>/_packaging/<your-feed-name>/pypi/simple`

In this case : `pip install dai-python-logging --extra-index-url https://pkgs.dev.azure.com/WBA/DAI/_packaging/DAI/pypi/simple`

- Step 3 : you can provide any username and  password (token)

![Scenario6](./docs/image6.png)


