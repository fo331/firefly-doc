﻿keywords: Task Properties, Options Tab, Query, Allow Query

Name in migrated code: **AllowBrowse**  
Location in migrated code: **OnLoad**


![Query](Query.png)

## Migrated Code Example


```csdiff   
protected override void OnLoad()
{
+    AllowBrowse = false;
}
``` 

Condition as an expression:

```csdiff   
protected override void OnLoad()
{
+     BindAllowBrowse(() => ENV.Security.UserManager.CurrentUser.Name == "SUPERVISOR");
}
```        
    



## Property Values
True or false. The default is **True** which is Allow Query = Yes in Magic
       