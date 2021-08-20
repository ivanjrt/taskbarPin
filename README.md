# Creating the shortcuts within a specific folder: (if a **lnk** file is created already then reference to that location)
* Regular apps create the shortcut</br>
  ![image](https://user-images.githubusercontent.com/44326428/130300937-b011d88d-ff93-44c1-972e-a8dd77a29554.png)

* For services and others: Right anywhere on desktop to create a shortcut </br>
  ![image](https://user-images.githubusercontent.com/44326428/130301050-bb5f96a4-1eac-4b60-80a4-0c625023bc83.png)
  
* To Invoke files with dependencies: create a shortcut sintax like so: program.exe "archivelocation.txt" </br>
![image](https://user-images.githubusercontent.com/44326428/130301274-b2ecd270-88f2-403f-a55f-44437cf9ef29.png)

# Creating a new Template: if you get it from a good resource </br>
or create your own from the same machine:</br>  
```
Export-StartLayout C:\Temp\layout2.xml
```
 # Re-Creating Template:</br>
 using VSCODE for excellent format retention: </br> 
 sample below but file attached. snippets don't handle xml very well </br>
 our main goal is edit our targets between the TaskBarPinList </br>
 ![image](https://user-images.githubusercontent.com/44326428/130301619-d2a58f25-2f7e-490c-a418-d9b081493ce7.png)

 At the end it should look like this, considering we have the path towards c:\temp </br>
 ![image](https://user-images.githubusercontent.com/44326428/130301959-2f93573b-bcf3-4132-a481-cb265b91ef4b.png)

# Applying the template: (Method 1. single Machine, This needs to be as Admin) </br>
 ```
 Import-StartLayout C:\Temp\layout.xml -MountPath c:\
 ```
 # Applying the template: (Method 2. GPO) </br>
 ![image](https://user-images.githubusercontent.com/44326428/130302215-af510ae8-c58e-4910-a712-dc4d2c717390.png)

# Applying the template: (Method 3. MDM -No tested) </br>
https://nathanblasac.com/deploy-a-custom-start-layout-configuration-policy-via-intune-windows-10-1809-a4ed72875c08

# Final Replication
Restart the system
  











