1.  In the AWS account I'm creating a bucket called “epam-simplesite” for this exercise

![](https://github.com/RonaldRengifoB/simplesite/blob/main/1.create-bucket.png?raw=true)

2\. Enabled Public Access to this bucket  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/2.enabled-public-access.png?raw=true)

3\. Set bucket versioning to "Disabled"  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/3.disabled-bucket-versioning.png?raw=true)

4\. set the default encryption and click on “Create bucket”  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/4.created-bucket.png?raw=true)

5\. As we can see the bucket is created  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/5.ev.png?raw=true)

6\. Edited the properties for website hosting

![](https://github.com/RonaldRengifoB/simplesite/blob/main/7.enabled-static-website.png?raw=true)

7\. In bucket properties, I enabled "Static website hosting", typed the name of the default webpage file “index.html” and Saved the changes
![](https://github.com/RonaldRengifoB/simplesite/blob/main/6.enable-hosting.png?raw=true)
  
8\. Created bucket policies.  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/8.added-bucket-policy.png?raw=true)

9\. Proceeded to create a user called “github” that will have full access to S3 buckets (we are going to use this user for GitHub actions)   
![](https://github.com/RonaldRengifoB/simplesite/blob/main/9.created-user-github.png?raw=true)

10\. Created access keys for the user  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/10-added-access-key.png?raw=true)

11\. Forked a GitHub repo containing an example index.html website  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/11.forked-repo-with-html.png?raw=true)

12\. Added the AWS credentials created in step (10) as repository secrets  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/12.added-keys-to-repo.png?raw=true)

13\. created the workflow to deploy the index.html in the repo to the bucket “epam-simplesite”  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/13-created-workflow.png?raw=true)

14\. Ran the workflow  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/14-ran-workflow.png?raw=true)

15\. Verified that the workflow ran successfully and that the website is visible with an AWS domain

http://epam-simplesite.s3-website-us-east-1.amazonaws.com  
![](https://github.com/RonaldRengifoB/simplesite/blob/main/15-site-running.png?raw=true)
