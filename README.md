<img src="https://imgix.datadoghq.com/img/dd_logo_n_70x75.png?ch=Width,DPR&fit=max&auto=format&w=70&h=75">


Run Synthetic Tests from Private Locations

Overview

Private locations allow you to monitor internal-facing applications or any private endpoints that aren’t accessible from the public internet.

https://datadog-docs.imgix.net/images/synthetics/private_locations/pl_view_file_1.808a2c3820f9b3e209bb98d9a63d3481.png?auto=format

We Configure private location by customizing the generated configuration file and this configuration file is in json format and we have stored this file in ssm parameter as it stores API key/Secret/Certificate. Now to fetch the ssm parameter inside cluster we are using secrets-store-csi-driver and mounting it to a pod for creating a secret with configuration file so DataDog agent can run with given configuration.
