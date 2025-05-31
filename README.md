# ts-installation-issues

when we use tsc command after ts installation ,
it could you face 

tsc : File C:\Users\UserName\AppData\Roaming\npm\tsc.ps1 cannot be loaded because running scripts is disabled on    
this system. For more information, see about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170.  
At line:1 char:1
+ tsc --version

# the cause 
because powerShell Excution Policy Does not Allow to run this scripts unless is relaxed
# the soltion 
1- Set-ExecutionPolicy RemoteSigned , by going to powerShell in Window Start and Run As Administrateur and write Set-ExecutionPolicy RemoteSigned and ansewr with Y
2-Select Command Prompt insteed of PowerShell 
