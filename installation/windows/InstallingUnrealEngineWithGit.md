# Installing Unreal Engine using Git

1. Open a PowerShell terminal by running it as administrator and change directory into the directory you want 
Unreal Engine to live.
2. In PowerShell, run:
    ```shell
    git clone -b <ENGINE_VERSION> --depth 1 --single-branch --filter=blob:none https://github.com/EpicGames/UnrealEngine.git
    ```
3. Once completed, run the following command - this will take a long time, possibly hours:
    ```shell
    .\Setup.bat && .\GenerateProjectFiles.bat
    ```
4. Open the `UE5.sln` and build the project - this will take some time.
5. Once complete, you can delete the `Binaries`, `Intermediate`, `Saved`, `.idea`, `.vs`, and `.sln` file from root directory
   of an Unreal project (NOT the in the UnrealEngine directory).
6. Right-click on the `.uproject` file > `Switch Unreal Engine version...` > choose the root directory of where you just
   installed Unreal Engine. This may also prompt you to generate files, in which case you should say yes to this.