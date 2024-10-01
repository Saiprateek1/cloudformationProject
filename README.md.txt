AWSTemplateFormatVersion: '2010-09-09'
Description: A CloudFormation template to create an S3 bucket with versioning enabled

Resources:
  MyS3Bucket:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: formation-s3-bucket-yaml-101-yourinitials-20230925
      VersioningConfiguration:
        Status: Enabled
      Tags:
        - Key: Project
          Value: MyAwesomeProject
        - Key: Environment
          Value: Development
