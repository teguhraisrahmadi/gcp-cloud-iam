# Google Cloud Platform

## Work Instruction for Create Custom Role in IAM

In this role I need permission for:
- resourcemanager.projects.get
- storage.buckets.list
- storage.multipartUploads.abort
- storage.multipartUploads.create
- storage.multipartUploads.list
- storage.multipartUploads.listParts
- storage.objects.create
- storage.objects.delete
- storage.objects.get
- storage.objects.list
- storage.objects.update

1. Go to IAM menu, and create custom role. 
<br> ![Capture](Material/1.png) <br>

2. Follow this option to fill the custom role permission. Then choose add permission.
<br> ![Capture](Material/2.png) <br>

3. Choose the permission based on list above this work instruction. Add this permission one by one.
<br> ![Capture](Material/3.png) <br>

4. Now we have 10 assigned permission for this role.
<br> ![Capture](Material/4.png) <br>

5. Then click create
<br> ![Capture](Material/5.png) <br>

6. Role was created.
<br> ![Capture](Material/6.png) <br>

Now we want to grant access for another google cloud account for our storage object resource based on custom role.

7. Go to IAM then click grant access.
<br> ![Capture](Material/7.png) <br>

8. Fill your another account. For this I am using another google account. Fill the “new principle” with your another account. Then assign role with custom role. And click save.
<br> ![Capture](Material/8.png) <br>

9. Now I go to another account to test this role. Now you can see, in another account it have the project one. Choose this and go to cloud storage.
<br> ![Capture](Material/9.png) <br>

10. Now I can access the cloud storage for this project.
<br> ![Capture](Material/10.png) <br>

11. I can go through in to the bucket too.
<br> ![Capture](Material/11.png) <br>

12. Done, Thanks.
