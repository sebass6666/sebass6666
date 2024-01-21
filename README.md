
git clone https://org.visualstudio.com/MyFirstProject/_git/MyFirstProject
Cloning into 'MyFirstProject'...
14:56:20.412270 ...\Common.cs:677       trace: [Main] git-credential-manager (v1.17.1) 'get'
14:56:20.484270 ...\Git\Where.cs:361    trace: [FindGitInstallations] found 1 Git installation(s).
14:56:20.492270 ...Configuration.cs:222 trace: [LoadGitConfiguration] git All config read, 20 entries.
14:56:20.497270 ...\Common.cs:547       trace: [LoadOperationArguments] http.proxy = 'http://proxy.company:8080'.
14:56:20.499270 ...tionArguments.cs:605 trace: [SetProxy] successfully set proxy to 'http://proxy.company:8080/'.
14:56:20.567270 ...\Common.cs:85        trace: [CreateAuthentication] detecting authority type for 'https://org.visualstudio.com/'.
14:56:20.587270 ...uthentication.cs:209 trace: [DetectAuthority] 'https://org.visualstudio.com/' is VSTS, tenant resource is {012345etc}.
14:56:20.589270 ...uthentication.cs:369 trace: [GetAuthentication] AAD authority for tenant '012345etc' detected.
14:56:20.679270 ...\Common.cs:132       trace: [CreateAuthentication] authority for 'https://org.visualstudio.com/' is Azure Directory.
14:56:20.909270 ...\Program.cs:603      trace: [Run] ! error: 'An error occurred while sending the request.'.
14:56:20.909270 ...\Program.cs:603      trace: [Run]        > 'The remote server returned an error: (407) Proxy Authentication Required.'.
14:56:20.915270 ...\Common.cs:642       trace: [LogEvent] System.Net.Http.HttpRequestException: An error occurred while sending the request. ---> System.Net.Web
Exception: The remote server returned an error: (407) Proxy Authentication Required.
   at System.Net.HttpWebRequest.EndGetResponse(IAsyncResult asyncResult)
   at System.Net.Http.HttpClientHandler.GetResponseCallback(IAsyncResult ar)
   --- End of inner exception stack trace ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Http.HttpClientWrapper.<GetResponseAsync>d__31.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Http.AdalHttpClient.<GetResponseAsync>d__22`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Http.AdalHttpClient.<GetResponseAsync>d__21`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.InstanceDiscovery.<DiscoverAsync>d__8.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.InstanceDiscovery.<GetMetadataEntryAsync>d__5.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Instance.Authenticator.<UpdateFromTemplateAsync>d__47.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Flows.AcquireTokenHandlerBase.<PreRunAsync>d__64.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Flows.AcquireTokenNonInteractiveHandler.<PreRunAsync>d__4.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.Internal.Flows.AcquireTokenHandlerBase.<RunAsync>d__57.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.AuthenticationContext.<AcquireTokenCommonAsync>d__37.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.IdentityModel.Clients.ActiveDirectory.AuthenticationContextIntegratedAuthExtensions.<AcquireTokenAsync>d__0.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at VisualStudioTeamServices.Authentication.Authority.<NoninteractiveAcquireToken>d__15.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at VisualStudioTeamServices.Authentication.AadAuthentication.<NoninteractiveLogon>d__4.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.Alm.Cli.CommonFunctions.<QueryCredentials>d__10.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.Alm.Cli.Program.<>c__DisplayClass23_1.<<Get>b__0>d.MoveNext()
14:56:20.981270 ...\Program.cs:603      trace: [Run] fatal: HttpRequestException encountered.
   An error occurred while sending the request.
fatal: HttpRequestException encountered.
   An error occurred while sending the request.
Username for 'https://org.visualstudio.com':
