<img src="https://imgix.datadoghq.com/img/dd_logo_n_70x75.png?ch=Width,DPR&fit=max&auto=format&w=70&h=75">


Run Synthetic Tests from Private Locations

Overview

Private locations allow you to monitor internal-facing applications or any private endpoints that aren’t accessible from the public internet.
Your private location worker pulls your test configurations from Datadog’s servers using HTTPS, executes the test on a schedule or on-demand, and returns the test results to Datadog’s servers. You can then visualize your private locations test results in a completely identical manner to how you would visualize tests running from managed locations.

<img src="https://datadog-docs.imgix.net/images/synthetics/private_locations/pl_view_file_1.808a2c3820f9b3e209bb98d9a63d3481.png">


Deployment Overview

Pod accesses the configuration file from the CSI Volume, which is provisioned by the CSI Driver that fetches the generated file from AWS SSM and then creates a secret from it inside the cluster and then datadog deployment uses that secret.

<img src="https://particule.io/images/aws-csi-secret-provider.png">


