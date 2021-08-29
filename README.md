# Windows-Process-Injection
C++ script to migrate your running process to another, by injecting your shell code into 64 bit process knowing its id. 

# Steps
  - Update the code by generating new msfvenom with your local address and local port, noting that the payload used for that code is windows/x64/meterpreter/reverse_tcp, after generating your venom update the "shellcode" variable with your venom. 
  - Compile the code using g++ inject.cpp -o inject.exe.
  - Upload your exe file to the target machine.
  - Configure the listner in new metasploit window.
  
    ![Screenshot 2021-08-29 171155](https://user-images.githubusercontent.com/48598374/131255463-c8d7a557-3822-47c5-885f-ff6c4a6a038d.png)
    
  - Choose the target process to which you would like to migrate.
  - run migrate.exe <process_id>

# Screenshots
![Screenshot 2021-08-29 172638](https://user-images.githubusercontent.com/48598374/131255984-5a881f80-8870-4a3d-b98a-c99e3ad3e1df.png)

![Screenshot 2021-08-29 172607](https://user-images.githubusercontent.com/48598374/131255990-c52251c8-ff79-46ac-84fc-9108e05a3fa6.png)
