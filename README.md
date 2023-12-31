---
metadata1: test
metadata2: metadata2
metadataArray:
  - test1
  - test2
---

###### OVERVIEW
# API Reference
The WorkOS API enables adding Enterprise Ready features to your application. This REST
API provides programmatic access and management of SSO, Magic Link, Directory Sync,
and Audit Trail resources.

[Sign in](#qwe) in to see code examples customized with your API keys and data.

```
https://api.workos.com
```
---
###### LANGUAGES
# Client Liabraries
WorkOS offers native SDKs in several popular programming languages. Choose one
language below to see our API Reference in your application’s language.

```java title="Test api liab !!!"
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.DeleteTicketingConnectionIdAgentIdRequest;
import com.Unified.Unified_to.models.operations.DeleteTicketingConnectionIdAgentIdResponse;
import com.Unified.Unified_to.models.operations.DeleteTicketingConnectionIdAgentIdSecurity;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            DeleteTicketingConnectionIdAgentIdRequest req = new DeleteTicketingConnectionIdAgentIdRequest("quibusdam", "unde");

            DeleteTicketingConnectionIdAgentIdResponse res = sdk.agent.deleteTicketingConnectionIdAgentId(req, new DeleteTicketingConnectionIdAgentIdSecurity("nulla") {{
                jwt = "";
            }});

            if (res.statusCode == 200) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

```html:TestTitle
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>I can haz embedded CSS and JS</title>
	<style>
		@media print {
			p { color: red !important; }
		}
	</style>
</head>
<body>
	<h1>I can haz embedded CSS and JS</h1>
	<script>
	if (true) {
		console.log('foo');
	}
	</script>

</body>
</html>
```
---
###### HOW TO CHECK
# Testing the API
The WorkOS API enables adding Enterprise Ready features to your application. This REST
API provides programmatic access and management of SSO, Magic Link, Directory Sync,
and Audit Trail resources.

~~Check out the guide about the WorkOS API Postman collection to learn more about it.~~

```
https://api.workos.com
```
