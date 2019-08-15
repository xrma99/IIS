# IIS publish .NET core (localhost) 
**（Both desktop and server OS）**

## Control Panel

- **Control Panel** >> **Programs** >> **Programs and Features** >> **Turn Windows features on and off**
- Select the whole **Internet Information Services**

## Publish VS project into **Folder**
> https://blog.csdn.net/qq_22642239/article/details/77006831 *添加网站* part.

## IIS manager

- In search box, search **inetmgr**, open the IIS manager
- Choose **Add Website...** 
- Name your website, choose the physical path and input a unique port number to your website.
- Click **OK**
> https://blog.csdn.net/zwk626542417/article/details/9796259 *3.网站发布* a&b part

## Change file permissions
> Please refer to [Microsoft Official Support File](https://support.microsoft.com/en-us/help/942055/http-error-500-19-error-when-you-open-an-iis-7-0-webpage) *HResultCode:0x80070005, Method 2*

BTW: To get computername, open cmd and input ***echo %computername%***

## Download 
- [.NET Core Hosting Bundle installer](https://www.microsoft.com/net/permalink/dotnetcore-current-windows-runtime-bundle-installer)
- [URL Rewrite](https://www.iis.net/downloads/microsoft/url-rewrite)
- [.NET Framework 4.8 Developer Pack](https://dotnet.microsoft.com/download/thank-you/net48-developer-pack)

## Run your website
- Open **IIS Manager**
- Double-click the only choice in left column
- Click **Sites**
- Click your website
- In right column, click **Browse \*:\[PortNumber](http)**


## Reference
Many thanks to:
- https://stackoverflow.com/questions/14132029/http-error-500-19-on-iis7-malformed-xml-in-web-config
- **https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/iis/?view=aspnetcore-2.2**
