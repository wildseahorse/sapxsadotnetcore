# sapxsadotnetcore
.Net core runtime 3.1 buildpack for SAP HANA XSA 2.0 SP4
All steps described below are tested with .Net Core Runtime 3.1.

Use the following scenario to create custom .Net runtime file for buildpack (runtime.tgz):

1. Download binary installer for .Net Core Runtime at https://dotnet.microsoft.com/download/dotnet-core or https://dotnet.microsoft.com/download/dotnet-core/3.1
2. Choose necessary package, here we use https://dotnet.microsoft.com/download/dotnet-core/thank-you/runtime-aspnetcore-3.1.5-linux-x64-binaries
3. Upload binary package file aspnetcore-runtime-3.1.5-linux-x64.tar.gz for ASP .Net Runtime Core 3.1.5 to the Linux HANA machine 
4. Create custom folder dotnet31 and unpack binary package with .Net Runtime (step 3) to that folder
5. Add necessary frameworks and assemblies to the folder dotnet31
6. Archive folder dotnet31 to create runtime.tgz file and place it to the buildpack folder ./runtime

To install the buildpack please follow the steps here https://www.youtube.com/watch?v=Ui4y1g3OqX4
