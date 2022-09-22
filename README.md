![Screenshot](dd_logo_n_70x75.png)


Run Synthetic Tests from Private Locations

Overview

Private locations allow you to monitor internal-facing applications or any private endpoints that aren’t accessible from the public internet.

![Screenshot](private-location.png)

<img src="https://imgix.datadoghq.com/img/dd_logo_n_70x75.png?ch=Width,DPR&fit=max&auto=format&w=70&h=75">

We Configure private location by customizing the generated configuration file and this configuration file is in json format and we have stored this file in ssm parameter as it stores API key/Secret/Certificate. Now to fetch the ssm parameter inside cluster we are using secrets-store-csi-driver and mounting it to a pod for creating a secret with configuration file so DataDog agent can run with given configuration.
