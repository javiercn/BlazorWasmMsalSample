# BlazorWasmMsalSample

Demonstrates how to replace the built-in AuthenticationService.ts file in the package with a custom implementation provided by the application. The example uses MSAL, but the steps are similar for Open ID Connnect.

## Steps:
* Install Microsoft.AspNetCore.ClientAssets
* Create an assets folder and copy all the files from https://github.com/dotnet/aspnetcore/tree/main/src/Components/WebAssembly/Authentication.Msal/src/Interop or https://github.com/dotnet/aspnetcore/tree/main/src/Components/WebAssembly/WebAssembly.Authentication/src/Interop except for the yarn.lock file.
* In `Index.html` replace the script `<script src="_content/.../AuthenticationService.js"></script>` with the one built by the application `<script src="AuthenticationService.js"></script>`
* You can now update the contents of AuthenticationService.ts within the assets folder to suit your scenarios.
