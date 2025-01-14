# github-demo2
# github-demo2


WinAppDriver v1.2.1 Latest
This is the first stable release in the v1.2 release cycle. It includes:

Improved compatibility with WebDriverIO
The ms:experimental-webdriver capability enables experimental features and optimizations - for this release, enabling this capability will provide performance improvements with XPath and improve overall element handling.
C#: appCapabilities.SetCapability("ms:experimental-webdriver", true);
The ms:waitForAppLaunch capability enables WinAppDriver to wait for a defined amount of time after an app launch is initiated prior to attaching to the application session. The limit for this is 50 seconds.
C#: appCapabilities.SetCapability("ms:waitForAppLaunch", "25"); to add app delay of 25 seconds.



In addition, there have been minimal changes from the v1.2 release candidate:

We've added retry logic to handle legacy applications that take a while to start up or display a splash screen.
We have improved support for packaged WinUI 3 Desktop applications. Please note: WinUI 3 is in preview.
As with the previous WinAppDriver v1.1 release, it is recommended that you use the WinAppDriver NuGet package to take full advantage of the advanced input with the Actions API.
