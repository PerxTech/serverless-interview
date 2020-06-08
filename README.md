# serverless interview
## Introduction
For this test, you will be working on a small piece of Perx architecture. When it comes to integrating our solution in our clients existing infrastructure. There are 2 possibilities, 
* real time using API
* by batch using a file upload

Real-time of course feels better but it might not be easy to achieve depending on our clients existing infrastructure.

This test focuses on the batch upload. 
> You need to build an AWS infrastructure which *automatically* picks-up new files from an s3 bucket and send the events to an sqs queue.

## Requirements
* It should support both csv or json files.
* For csv, it should generate one event per row.
* For json, if the content is an array, it should send one event per array item, otherwise it should send just one event.
* You can use any aws service, lambda, step functions, ...
* For the infrastructure code, you can use any of cloud formation, sam, serverless or terraform.
* If you write some lambda code, you can use any language supported by lambda.
* The setup of the s3 bucket and the sqs queue should be part of the deliverable.

## Deliverable
You need to provide us a link to a repository which contains both the infrastructure code and the eventual serverless code.
