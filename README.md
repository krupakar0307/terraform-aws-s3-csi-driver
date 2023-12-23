<h1 align="left" id="title">terraform-eks-s3-csi-mount</h1>

<p id="description">This module is used to install eks s3-csi driver in eks cluster.</p>

<h2>🛠️ Installation Steps:</h2>

Initially, set up an S3 Bucket, integrate the below module into your code, and either create a variables file containing mapped strings or directly input values instead of using var.s3_csi_inputs.*</p>


```
module "eks-s3-csi" {
  source           = "krupakar0307/s3-csi-driver/aws"
  version          = "0.0.2"
  aws_region       = "region"
  aws_profile     = "profile_name"
  bucket_name   = "bucket_name"
  iam_role_name    = "role_name"
  eks_cluster = "cluster_name"
}
```
