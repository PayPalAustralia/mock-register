## Getting Started
This file contains the steps to run and debug this project in a MacOS development environment:

- Download and install dotnet 5 for MacOS.
- Set the environment variable ASPNETCORE_ENVIRONMENT to Development.
- Import the Mock CDR CA cert (Source/CDR.Register.API.Gateway.mTLS/Certificates/ca.crt) with KeyChain Access from MacOS and set it to Always Trust.
- Update the path for databases and logs for: 
    * Source/CDR.Register.Admin.API/appsettings.Development.json (replace with Source/CDR.Register.Admin.API/appsettings.Development.MAC.json)
    * Source/CDR.Register.Discovery.API/appsettings.Development.json (replace with Source/CDR.Register.Discovery.API/appsettings.Development.MAC.json)
    * Source/CDR.Register.IdentityServer/appsettings.Development.json (replace with Source/CDR.Register.IdentityServer/appsettings.Development.MAC.json)
    * Source/CDR.Register.SSA.API/appsettings.Development.json (replace with Source/CDR.Register.SSA.API/appsettings.Development.MAC.json)
    * Source/CDR.Register.Status.API/appsettings.Development.json (replace with Source/CDR.Register.Status.API/appsettings.Development.MAC.json)
- Run Source/Start-Register.sh to start all the sub-projects (you may need to install ttab https://github.com/mklement0/ttab).