# Cloud-Storage-Qwik-Start---Google-Cloud-Console
Cloud Storage allows world-wide storage and retrieval of any amount of data at any time. You can use Cloud Storage for a range of scenarios, such as serving website content, storing data for archival and disaster recovery, or distributing large data objects to users via direct download.

In this hands-on lab you will learn how to use the Cloud console to:

** Create a storage bucket
** Upload objects to the bucket
** Create folders and subfolders in the bucket
** Make objects in a storage bucket publicly accessible


Task 1. Create a bucket
Buckets are the basic containers that hold your data in Cloud Storage.

To create a bucket:

In the Cloud console, go to Navigation menu (Navigation menu) > Cloud Storage > Buckets.

Click + Create.

 Cloud Console Storage Browser. Create Bucket button is highlighted.

Enter your bucket information and click Continue to complete each step:

Name your bucket: Enter a unique name for your bucket. For this lab, you can use your Project ID as the bucket name because it will always be unique.
Bucket naming rules:

Do not include sensitive information in the bucket name, because the bucket namespace is global and publicly visible.

Bucket names must contain only lowercase letters, numbers, dashes (-), underscores (_), and dots (.). Names containing dots require verification.

Bucket names must start and end with a number or letter.

Bucket names must contain 3 to 63 characters. Names containing dots can contain up to 222 characters, but each dot-separated component can be no longer than 63 characters.

Bucket names cannot be represented as an IP address in dotted-decimal notation (for example, 192.168.5.4).

Bucket names cannot begin with the "goog" prefix. Bucket names cannot contain "google" or close misspellings of "google".*

Also, for DNS compliance and future compatibility, you should not use underscores (_) or have a period adjacent to another period or dash. For example, ".." or "-." or ".-" are not valid in DNS names.

Choose Region for Location type and asia-southeast1 for Location.

Choose Standard for Set a default class.

Choose Uniform for Access control and uncheck Enforce public access prevention on this bucket to turn it off.

Leave the rest of the fields as their default values and click Create.

That's it — you've just created a Cloud Storage bucket!

Note: If you are prompted with Public access will be prevented, uncheck Enforce public access prevention on this bucket and click Confirm.
Test completed task
Click Check my progress to verify your performed task. If you have successfully created a Cloud Storage bucket, you will see an assessment score.

Assessment Completed! Bucket count: 1. Bucket name(s): ["qwiklabs-gcp-03-54af8cd9a4ed"]
Create a bucket
Assessment Completed! Bucket count: 1. Bucket name(s): ["qwiklabs-gcp-03-54af8cd9a4ed"]
Test your understanding
Below are multiple choice questions to reinforce your understanding of this lab's concepts. Answer them to the best of your ability.


Every bucket must have a unique name across the entire Cloud Storage namespace.
check
True
False



Task 2. Upload an object into the bucket
A cute fluffy kitten

To upload the image above into your new bucket:

Right-click the kitten.png image in this section and download it to your computer. Save the image as kitten.png, renaming it on download.

In the Cloud Storage browser page, click the name of the bucket that you created.

In the Objects tab, click Upload > Upload files.

In the file dialog, go to the file that you downloaded and select it.

Ensure the file is named kitten.png. If it is not, click the three dot icon for your file, select Rename from the dropdown, and rename the file to kitten.png.

After the upload completes, you should see the file name and information about the file, such as its size and type.

Test completed task
Click Check my progress to verify your performed task. If you have successfully uploaded an object to your bucket, you will see an assessment score.

Assessment Completed! Bucket name(s): ["qwiklabs-gcp-03-54af8cd9a4ed"] Object count: [1]
Upload an object into the bucket (kitten.png)
Assessment Completed! Bucket name(s): ["qwiklabs-gcp-03-54af8cd9a4ed"] Object count: [1]
Test your understanding
Below are multiple choice questions to reinforce your understanding of this lab's concepts. Answer them to the best of your ability.


Object names must be unique only within a given bucket.
check
True
close
False

Task 3. Share a bucket publicly
To allow public access to the bucket and create a publicly accessible URL for the image:

Click the Permissions tab.

Ensure the view is set to View by principals tab. Click Grant access to view the Add principals pane.

In the New principals box, enter allUsers.

In the Select a role drop-down, select Cloud Storage > Storage Object Viewer.

Click Save.

In the Are you sure you want to make this resource public? window, click Allow public access.

Test completed task
Click Check my progress to verify your performed task. If you have successfully shared an object publicly from your bucket, you will see an assessment score.


Share a kitten.png object publicly

To verify, click the Objects tab to return to the list of objects. Your object's Public access column should read Access granted to public principals.
Note: If your object does not appear to be public after following the previous steps, you may need to refresh your browser page.
Press the Copy URL button for your object and paste it into a separate tab to view your image.
The Copy URL button provides a shareable URL similar to the following:

https://storage.googleapis.com/YOUR_BUCKET_NAME/kitten.png


Task 4. Create folders
In the Objects tab, click Create folder.

Enter folder1 for Name and click Create.

You should see the folder in the bucket with an image of a folder icon to distinguish it from objects.

Create a subfolder and upload a file to it:

Click folder1.

Click Create folder.

Enter folder2 for Name and click Create.

Click folder2.

Click Upload > Upload files.

In the file dialog, navigate to the screenshot that you downloaded and select it.

After the upload completes, you should see the file name and information about the file, such as its size and type.



Task 5. Delete a folder
Click the arrow next to Bucket details to return to the buckets level.

Select the bucket.

Click on the Delete button.

In the window that opens, type DELETE to confirm the deletion of the folder.

Click Delete to permanently delete the folder and all objects and subfolders in it.
