# codedeploy


{
 "Version": "2012-10-17",
 "Statement": [
  {
    "Effect": "Allow",
    "Action": [
      "logs:*"
    ],
    "Resource": "arn:aws:logs:*:*:*"
  },
  {
    "Effect": "Allow",
    "Action": [
      "s3:GetObject"
    ],
    "Resource": [
      "arn:aws:s3:::BUCKET_NAME/*"
    ]
  },
  {
    "Effect": "Allow",
    "Action": "codedeploy:GetDeploymentConfig",
    "Resource": "arn:aws:codedeploy:us-east-1:123ACCOUNTID:deploymentconfig:*"
  },
  {
    "Effect": "Allow",
    "Action": "codedeploy:RegisterApplicationRevision",
    "Resource": "arn:aws:codedeploy:us-east-1:123ACCOUNTID:application:*"
  },
  {
    "Effect": "Allow",
    "Action": "codedeploy:GetApplicationRevision",
    "Resource": "arn:aws:codedeploy:us-east-1:123ACCOUNTID:application:*"
  },
  {
    "Effect": "Allow",
    "Action": "codedeploy:CreateDeployment",
    "Resource": "arn:aws:codedeploy:us-east-1:123ACCOUNTID:deploymentgroup:*"
   }
 ]
}
