# Azure_AI_Engineer_Demos
A series of notebook I created while preparing for the AI-102 Azure AI Engineer Associate exam.

## Prerequisites
- Make sure to use the `Azure_Utils` [package](https://github.com/benoitchamot/Azure_Utils):

```bash
cd "path_to_this_project"
git clone https://github.com/benoitchamot/Azure_Utils.git
```

- Prepare your Azure subscription with the necessary resources for the AI Services
- Store all your credentials in a Secrets Vault in your Azure subscription
- Install [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/) to log in to your subscription
- The notebooks include commands to install the necessary packages but some other dependencies may be required depending on your environment
- A `.env` file must be created to store the endpoints URLs, secrets names and other parameters (please refer to the notebooks for more details)

The `.env` variables are loaded with `dotenv`:

```python
import os
from dotenv import load_dotenv

# Load environment variables from file
load_dotenv()

# Get environment variables
VISION_ENDPOINT = os.getenv('VISION_ENDPOINT')

# Your code here...
```

## Disclaimer
This repository provides example notebooks for using Azure AI services via the Azure Python SDK. The code is provided as-is, without warranty, and may not reflect the latest Azure features or SDK updates. Users are solely responsible for resource provisioning, associated costs, and ensuring the security of their Azure accounts.