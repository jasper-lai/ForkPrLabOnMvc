## 專案採用 SDK 6.0.403 版

因為 SDK 被改為 7.0.100, 所以若要改回 6.0.403, 要額外作處理  

```powershell
PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> dotnet --list-sdks
2.1.202 [C:\Program Files\dotnet\sdk]
2.1.403 [C:\Program Files\dotnet\sdk]
2.1.526 [C:\Program Files\dotnet\sdk]
3.0.100 [C:\Program Files\dotnet\sdk]
3.1.302 [C:\Program Files\dotnet\sdk]
5.0.414 [C:\Program Files\dotnet\sdk]
6.0.403 [C:\Program Files\dotnet\sdk]
7.0.100 [C:\Program Files\dotnet\sdk]

PS D:\22-Projects.Git\52-ASP.NET Core> mkdir ApiLab6.0  

PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> dotnet new globaljson  
範本「global.json 檔案」已成功建立。  

PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> notepad global.json

PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> type global.json  
{
  "sdk": {
    "version": "6.0.403"
  }
}

PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> dotnet new --list
這些範本符合您的輸入:

範本名稱                                      簡短名稱             語言        標記
--------------------------------------------  -------------------  ----------  -------------------------------------
方案檔                                        sln,solution                     Solution
主控台應用程式                                console              [C#],F#,VB  Common/Console
類別庫                                        classlib             [C#],F#,VB  Common/Library
ASP.NET Core Empty                            web                  [C#],F#     Web/Empty
ASP.NET Core gRPC Service                     grpc                 [C#]        Web/gRPC
ASP.NET Core Web API                          webapi               [C#],F#     Web/WebAPI
ASP.NET Core Web App                          webapp,razor         [C#]        Web/MVC/Razor Pages
ASP.NET Core Web App (Model-View-Controller)  mvc                  [C#],F#     Web/MVC
ASP.NET Core with Angular                     angular              [C#]        Web/MVC/SPA
ASP.NET Core with React.js and Redux          reactredux           [C#]        Web/MVC/SPA

PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> dotnet new webapi
範本「ASP.NET Core Web API」已成功建立。

正在處理建立後的動作...
正在 D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0\ApiLab6.0.csproj 上執行 'dotnet restore'...
  正在判斷要還原的專案...
  已還原 D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0\ApiLab6.0.csproj (307 ms 內)。
還原成功。

PS D:\22-Projects.Git\52-ASP.NET Core\ApiLab6.0> code .

```


