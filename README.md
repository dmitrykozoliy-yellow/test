###### OVERVIEW
# API Reference
The WorkOS API enables adding Enterprise Ready features to your application. This REST
API provides programmatic access and management of SSO, Magic Link, Directory Sync,
and Audit Trail resources.

[Sign in](#qwe) in to see code examples customized with your API keys and data.


* [deleteTicketingConnectionIdAgentId](#deleteticketingconnectionidagentid) - Remove a agent
* [getTicketingConnectionIdAgent](#getticketingconnectionidagent) - List all agents
* [getTicketingConnectionIdAgentId](#getticketingconnectionidagentid) - Retrieve a agent
* [getUcConnectionIdAgent](#getucconnectionidagent) - List all agents
* [patchTicketingConnectionIdAgentId](#patchticketingconnectionidagentid) - Update a agent
* [postTicketingConnectionIdAgent](#postticketingconnectionidagent) - Create a agent
* [putTicketingConnectionIdAgentId](#putticketingconnectionidagentid) - Update a agent

## deleteTicketingConnectionIdAgentId

Remove a agent

## Example Usage

```java
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

