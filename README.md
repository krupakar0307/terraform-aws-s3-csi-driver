<h1 align="left" id="title">terraform-eks-s3-csi-mount</h1>

<p id="description">This module is used to install eks s3-csi driver in eks cluster.</p>

<h2>🛠️ Installation Steps:</h2>

Initially, set up an S3 Bucket, integrate the below module into your code, and either create a variables file containing mapped strings or directly input values instead of using var.s3_csi_inputs.*</p>


```
module "eks-s3-csi" {
  source           = "krupakar"
  aws_profile      = "your_profile_name"
  aws_region       = "region"
  s3_bucket_name   = "bucker_name"
  iam_role_name    = "role_name"
  eks_cluster_name = "cluster_name"
}
```