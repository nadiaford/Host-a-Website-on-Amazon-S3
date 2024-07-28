# Host a Website on Amazon S3
## Overview
I used AWS S3 aka (Amazon Simple Storage Service) to host a website. It is used to store and retrieve any amount of data at any time from anywhere on the web.
<br />

#### Static website hosting means...
a site is delivered to the user exactly the way it's stored with the code and assest files.
<br />

#### In AWS, I enabled static website hosting by...
enabling site for web hosting and by making the files public using ACL (Access Control Lists).

#### One thing I didn't expect...
Is how easy it was to do this. It took me 30 minutes to complete this project.

<br />


## Project Walk-Through

### 1️⃣ Create an S3 Bucket
Creating an S3 Bucket took me no time to complete this task. No more than 3 minutes.

#### My Region configurations:
US-east-1 (N. Virginia) because I'm based in Maryland.
<br />

#### My Access Control List configurations:
ACL is a set of rules that decides who gets access to which resources within AWS.
<br />

#### S3 bucket naming is important!
No other AWS account in the entire world can use your bucket's name unless you delete the bucket
<br /><br />

<img src="https://i.imgur.com/hfBrP3q.png" height="80%" width="80%" alt="AWS S3 Bucket"/>
<br />

### 2️⃣ Upload Website Files to S3
Next, I uploaded the following files: index.html and NextWork - Everyone should be in a job they love_files.
<br />

#### How these files work...
The index.html file is the front end code that is necessary to visually present the website. The folder had all of the assests needed to add to the designs, ie fonts, media, backend code(JavaScript).
<br /><br />

<img src="https://i.imgur.com/MAuy6WM.png" height="80%" width="80%" alt="File Upload"/>
<br /><br />

### 3️⃣ Static Website Hosting on S3
Static website hosting is website hosting is what makes your website public on the internet.
<br />
#### How I enabled hosting...
Go to the "Properties" tab, scroll down to the "Static Website Hosting" section, edit the settings, and configured the settings to enable the web hosting to static to reference the index.html file.
<br /><br />
<img src="https://i.imgur.com/tXSzJK6.png" height="80%" width="80%" alt="Static Website Hosting S3"/>
<br /><br />

### 4️⃣ Bucket Endpoints

#### Bucket Endpoint URLs
The url provides a publicly used address to access the website.
<br /></br >
<img src="https://i.imgur.com/AL2VKBK.png" height="80%" width="80%" alt="Make Files Public"/>
<br /><br />

### 5️⃣ An error!
When I first visited the bucket endpoint URL, I saw was met with a 404 error code.
<br />

#### Why did I get an error?
The error message is saying that your static website is being hosted by S3, but the actual HTML/image files you've uploaded are still private. To solve this error, we need to set the permission of the objects to public.
<br /><br />
<img src="https://i.imgur.com/xoQOs1s.png" height="80%" width="80%" alt="404 Error"/>
<br /><br />

### 6️⃣ Success 🎉
To solve this error, we need to set the permission of the objects to public.
<br /><br />
<img src="https://i.imgur.com/OklV05W.png" height="80%" width="80%" alt="Success Status"/>
<br /><br />
