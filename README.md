# Launching and Managing a Web Application with AWS CloudFormation

In this lab , you learn how to use AWS Cloud Formation to provision andupdate a web application with a number of supporting AWS productsand services , including Auto Scaling groups , Amazon Elastic ComputeCloud ( EC2 ) instances , and Elastic Load Balancing


In the first part you create a simple resource , an Amazon s3 bucketwith AWS Cloudformation and you look at different retention policiesapplied when you delete an AWS Cloud


In the second part , you provision a simple PHP web application usingan Amazon Linux instance . You then see how to re-apply an AWSCloudformation template to the existing application to change someesource attributes such as an Amazon EC2 instance type . Finally , youadd a load balancer and an Auto Scaling group based on an AutoScaling confiquration

# Topics covere

By the end of this lab , you are able to:

  * Create an Amazon Simple Storage Service ( S3 ) bucket using AWSCloudformation

  * Provision a simple PHP web application using an Amazon Linux AMI

  * Apply an AWS Cloud Formation template to an existing application

  * Modify an existing application using AWS Cloud Formatio

  * Add LAM roles and Elastic Load Balancing to the application usingAWS Cloud Formation


 # Technical Knowledge prerequisites

 To successfully complete this lab , you need to be comfortable editingscripts in a text editor


 # Other AWS Services


 The IAM policy assigned to your lab user prohibits the use of AWSservices not included in this ab In some cases . imitations extendbeyond this restriction as an intentional aspect of the lab desigxpect errors when accessing other services or performing actionsbeyond those provided in this lab guide


 AWS Cloudformation gives developers and systems administrators aneasy way to create and manage a collection of related AWS resources ,provisioning and updating them in an orderly and predictable fashion


You can use AWS Cloudformation sample templates or create yourown templates to describe the AWS resources , and any associateddependencies or runtime parameters , required to run your applicationYou don't need to figure out the order for provisioning AWS services orthe subtleties of making those dependencies work . AWSCloudformation takes care of this for you . After the AWS resourcesare deployed you can modify and update them in a controlled andpredictable way , in effect applying version control to your AWSinfrastructure the same way you do with your software


You can deploy and update a template and its associated collection oresources ( called a stack ) by using the AWS Management ConsoleAWS Command Line Interface or Apls . AWS Cloudformation isavailable at no additional charge , and you pay only for the AWSresources needed to run your applications


An AWS Cloud Formation template is a declaration of the AWSresources that make up a stack . The template is stored as a text file ineither Javascript Object Notation ( JSON ) or YAML format . Becausethey are just text files , you can create and edit them in any text editorand manage them in your source control system with the rest of yoursource code


In the templates for this lab , you use the YAML structure that AWSCloudformation can interpret to declare the AWS resources you wantto create and configure . In the YAML format , an obiect is declared as aname-value pair or a pairing of a name . In an AWS Cloudformatiotemplate you can declare the following six top-level objects


  * AWStemplateformatVersion
  * Description
  * Parameters
  * Mappings
  * Resources
  * Outputs


The only required top-level object is the Resources object , which mustdeclare at east one resource This lab starts with the most basictemplate containing only a Resources object , which contains a singleresource declaration


Definitions of each of these obiects can be found in the online [Template Anatomy](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-anatomy.html#concept-template-description) documentation


# Start lab


1. to launch the lab , at the top of the page , choose Start Lab


If you are prompted for a token , use the one distributed to you ( orcredits you have purchased










