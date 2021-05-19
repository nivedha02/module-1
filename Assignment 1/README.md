# module-2
Maintain Efficient Process Utilization on Windows:

### Collect process information using the Task Viewer:

In this assignment we gonna terminate a process with commands.ok,let's dive into....
             
#### loaction: on search --> task manager --> PRESS ENTER .The snap below will be seen .            
![Screenshot (574)](https://user-images.githubusercontent.com/76787422/118834008-898eff80-b8df-11eb-8996-793e19e72178.png)


Move to details on the top ,you can able to see all the details about the current running processes.

![Screenshot (578)](https://user-images.githubusercontent.com/76787422/118834075-957ac180-b8df-11eb-99d8-a37e0a6012ca.png)

### Terminate a specific process using Windows PowerShell:

### loaction: on search -->windows powershell--> PRESS ENTER

To view the task process in powershell get-process is used.
     
      get-process
      
All the running processes will be listed below.
![Screenshot (575)](https://user-images.githubusercontent.com/76787422/118840094-b396f080-b8e4-11eb-858e-eea510d0f799.png)

  
taskkill is used to terminate a process in windows.
     
     taskkill /f /pid (process identifier)

/f- Is used to force the action

/pid- Is generated automatically when a process is begins and it is UNIQUE!!!!!

![Screenshot (603)](https://user-images.githubusercontent.com/76787422/118843205-754f0080-b8e7-11eb-9333-87bf1669dac4.png)

We can terminate a process with PID(process identifier) (or) with IM(image name).PID of every tab on your browser is different but the IM(image name) for a browser will be same that is chrome.exe for google chrome.
we can able to see the IM(image name) or PID(process id) of a process with the details section on the task manager or else, we can also use the get-process as seen before.
   
    taskkill /f /im (image name of a process like chrome.exe)
    
![Screenshot (605)](https://user-images.githubusercontent.com/76787422/118843659-e55d8680-b8e7-11eb-921e-37d5108ac3bc.png)




### Multiple processes termination:

In multiple process termination two or more processes are terminated at once.

       taskkill /f /pid (one pid) /pid (other pid)

![Screenshot (600)](https://user-images.githubusercontent.com/76787422/118845125-21ddb200-b8e9-11eb-95c4-6d54668b928b.png)

       taskkill /f /im (one im) /im (other im)
       
![Screenshot (598)](https://user-images.githubusercontent.com/76787422/118845269-420d7100-b8e9-11eb-97fc-634efa38f1e8.png)

cheers,we completed :blush: :blush: 
