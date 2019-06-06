# Try Out VS Cloud Environments: .NET Core

This is a sample project that lets you try out VS Cloud Environments in a few easy steps.
   
## Things to try

This sample has been cloned into your VS Cloud Environment. You're able to work with it like you would any local code.

Some things to try:

1. **Terminal:** 
  - Press ctrl+shift+[backtick] to open the terminal
  - From the terminal run `dotnet --version`
    > Note: dotnet is not installed on the local machine, yet you're able to use it! 
  - Type other Linux commands (`uname`, `ls`, etc.) to interact with the underlying environment

2. **Use dotnet:** 
  - Restore NuGet packages
  - Press `ctrl+shift+B` to run the build task

3. **Edit code:**
   - Open `Program.cs`
   - Try adding some code and check out the IntelliSense

4. **Build, Run, and Debug:**
   - Open `Program.cs`
   - Change the message to "Hello {your name} from ASP.NET Core!"
   - Add a breakpoint (e.g. on line 21).
   - Press F5 to launch the app
   - Once the breakpoint is hit, try hovering over variables, examining locals, and other debugging tasks
   - Continue, then open a local browser and go to `http://localhost:9000`.

5. **Forward port:**
   - Stop debugging and remove the breakpoint.
   - Open `Program.cs`
   - Change the server port to 5000. (`.UseUrls("http://0.0.0.0:5000")`)
   - Press F5 to launch the app in the container.
   - Run the **Cloud Environments: Forward Port from Environment...** command
     - Enter port 5000
     - Name it anything you'd like
     - View the forwarded ports in the Environment Details panel
   - Open the local browser and go to http://localhost:5000/ to see the app running on a different port.

6. **Source Control:**
    - From the Source Control side bar:
      - Stage changes.
      - Commit changes.
      - Push changes.