<img src="https://imgix.datadoghq.com/img/dd_logo_n_70x75.png?ch=Width,DPR&fit=max&auto=format&w=70&h=75">


Run Synthetic Tests from Private Locations

Overview

Private locations allow you to monitor internal-facing applications or any private endpoints that aren’t accessible from the public internet.

<img src="https://datadog-docs.imgix.net/images/synthetics/private_locations/pl_view_file_1.808a2c3820f9b3e209bb98d9a63d3481.png">


Pod stores the configuration file which we have generated above from the CSI Volume, which is provisioned by the CSI Driver that fetches the Secret content from AWS SSM and then creates a secret from it inside the cluster and then datadog deployment use that secret.

<img src="https://particule.io/images/aws-csi-secret-provider.png">


