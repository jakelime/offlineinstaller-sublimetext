# Offline installer - SublimeText

An offline installer for sublimetext

## Hook `subl` to powershell

1. locate $profile using powershell

   ```powershell
   (base) PS C:\Users\70014156> $profile
   C:\Users\jakelime\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
   ```

1. Add the following function into `PowerShell_profile.ps1`

   ```powershell
   # C:\Users\jakelime\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
   function subl ($arg){
       & 'C:\Users\70014156\AppData\Local\SublimeText\subl.exe' $arg
   }
   echo "custom functions loaded - @jakelime"
   ```
   
   
