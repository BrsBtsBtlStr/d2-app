# d2-app
Simple application that queries various game data from Bungie's API.

## Installation & Setup:
1. Create and register your new application by navigating to https://www.bungie.net/en/Application
    > *OAuth Client Type = "Confidential"*

2. Copy and save down the follwing credentials/endpoints from the 'app details page'
    * API Key
    * Client Id
    * Client Secret
    * Authorization Url

3. Clone git repo: https://github.com/BrsBtsBtlStr/d2-app

4. Create an '.env' file like the code below and save in the cloned repo from last step. 
    ```
    CLIENT_ID = 'enter your CLIENT_ID'
    CLIENT_SECRET = 'enter your CLIENT_SECRET'
    API_KEY = 'enter your API_KEY'
    ```

    >_Note: the purpose of creating and using this .env file is to protect sensitive information like the user's client id, client secret, and api key. The d2-api-app.py script will pull these values from the .env file without giving away sensitive info. The user doesn't have to worry about accidentally publishing their api key to a public GitHub repo. The .gitignore file instructs GitHub to exclude this file from publishing to the repo._

5. Setup the working environment:
    **For anaconda distributions:**

        ```
        conda create -n d2env python:3.9 anaconda
        conda activate d2env
        conda install -c anaconda d2env
        ```
    **For python3:**

        ```
        python3 -m venv d2env
        source d2env/bin/activate
        pip3 install requests requests-oauthlib python-dotenv
        ```

6. Now run the program: 
    >d2-api-app.py

## Roadmap:

- [x] Custom redirect webpage created
- [x] API connection established
- [ ] API endpoints identified
- [ ] Crucible stat tracker
- [ ] Armor picker
- [ ] Build creator


## How to use:
 _Coming soon..._


