# Creating an Amazon Virtual Private Cloud (VPC) with AWS CloudFormation

This lab shows how to create an Amazon Virtual Private Cloud(VPC)using AWS Cloudformation

Using AWS Cloudformation is an excellent way to deploy VPCS in areliable, repeatable manner because the template used by Cloudformation acts as documentation to show exactly what is beingdeployed

You walkthrough the sections of an AWS Cloudformation templateand examine the resources that are deployed. You also learn how toperform updates through Cloudformation


# Topics covered

In this lab you:


  * Deploy an AWS Cloudformation template that creates an AmazonVPC

  * Examine the components of the template

  * Update a Cloudformation stack

  * Examine a template with the AWS Cloudformation DesignerDelete a Cloudformation stack


# AWS Cloudformation


AWS Cloudformation gives developers and systems administrators aneasy way to create and manage a collection of related AWS resources ,provisioning and updating them in an orderly and predictable fashion

You can use AWS Cloudformation's sample templates or create yourown templates to describe the AWS resources , and any associateddependencies or runtime parameters , required to run your applicationYou don't need to figure out the order for provisioning AWS services othe subtleties of making those dependencies work . Cloudformationtakes care of this for you . After the AWS resources are deployed , youcan modify and update them in a controlled and predictable way ,effect applying version control to your AWS infrastructure the sameway you do with your software


You can deploy and update a template and its associated collection ofresources ( called a stack ) by using the AWS Management ConsoleAWS Command Line Interface or Apls . Cloudformation is available atno additional charge , and you pay only for the AWS resources neededto run your applications


# Amazon Virtual Private Cloud ( VPC )


Amazon Virtual Private Cloud ( Amazon VPC ) lets you provision alogically isolated section of the AWS cloud where you can launchresources within a virtual network . You have complete control oveyour virtual networking environment , including selection of your ownP address range , creation of subnets , and confiquration of routetables and network gateways


You can easily customize the network configuration for your virtualprivate cloud . For example , you can create a public-facing subnet foiour web servers that has access to the Internet and place youbackend systems such as databases or application servers in aprivate-facing subnet with no Internet access . You can leveragemultiple layers of security , including security groups and networkaccess control lists , to help control access to Amazon EC2 instancesn each subnet



# Task 1: Deploy a Stack using AWSCloudformation

In this task , you deploy a pre-defined Cloud Formation template to buildan Amazon VPC

3. Download the [vpc-1](https://amazon.qwiklabs.com/focuses/53930?parent=catalog) yaml Cloudformation template to yourcomputer


You examine the contents of the template in the next task


4. At the top of the AWS Management Console , in the search bar ,search for and choose Cloudformation













