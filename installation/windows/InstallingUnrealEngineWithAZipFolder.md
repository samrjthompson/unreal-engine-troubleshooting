# Installing Unreal Engine using a ZIP folder

1. Go to https://github.com/EpicGames/UnrealEngine.
2. Choose the engine version you want from the branches.
3. Click `Code` and `Download ZIP`.
4. Once the ZIP folder has downloaded, change the name of it from `UnrealEngine-X.X.zip` to `UnrealEngine.zip`.
5. Extract the contents to your desired location.
6. Once the extraction has completed, open a PowerShell by running it as administrator, and `cd` into the `UnrealEngine` 
directory that was created.
7. In the PowerShell terminal, run the following command:
    ```shell
    .\Setup.bat && .\GenerateProjectFiles.bat
    ```
8. Open the `UE5.sln` and build the project - this will take some time.
9. Once complete, you can delete the `Binaries`, `Intermediate`, `Saved`, `.idea`, `.vs`, and `.sln` file from root directory 
of an Unreal project (NOT the in the UnrealEngine directory). 
10. Right-click on the `.uproject` file > `Switch Unreal Engine version...` > choose the root directory of where you just
installed Unreal Engine. This may also prompt you to generate files, in which case you should say yes to this.