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

### Example Usage

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

### Parameters

| Parameter                                                                                                                                                    | Type                                                                                                                                                         | Required                                                                                                                                                     | Description                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                    | [com.Unified.Unified_to.models.operations.DeleteTicketingConnectionIdAgentIdRequest](../../models/operations/DeleteTicketingConnectionIdAgentIdRequest.md)   | :heavy_check_mark:                                                                                                                                           | The request object to use for the request.                                                                                                                   |
| `security`                                                                                                                                                   | [com.Unified.Unified_to.models.operations.DeleteTicketingConnectionIdAgentIdSecurity](../../models/operations/DeleteTicketingConnectionIdAgentIdSecurity.md) | :heavy_check_mark:                                                                                                                                           | The security requirements to use for the request.                                                                                                            |


### Response

**[com.Unified.Unified_to.models.operations.DeleteTicketingConnectionIdAgentIdResponse](../../models/operations/DeleteTicketingConnectionIdAgentIdResponse.md)**


## getTicketingConnectionIdAgent

List all agents

### Example Usage

```java
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentRequest;
import com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentResponse;
import com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentSecurity;
import java.time.LocalDate;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            GetTicketingConnectionIdAgentRequest req = new GetTicketingConnectionIdAgentRequest("corrupti") {{
                limit = 8472.52d;
                offset = 4236.55d;
                order = "error";
                query = "deserunt";
                sort = "suscipit";
                updatedGte = LocalDate.parse("2022-09-14");
            }};            

            GetTicketingConnectionIdAgentResponse res = sdk.agent.getTicketingConnectionIdAgent(req, new GetTicketingConnectionIdAgentSecurity("debitis") {{
                jwt = "";
            }});

            if (res.ticketingAgents != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                                                          | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                          | [com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentRequest](../../models/operations/GetTicketingConnectionIdAgentRequest.md)   | :heavy_check_mark:                                                                                                                                 | The request object to use for the request.                                                                                                         |
| `security`                                                                                                                                         | [com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentSecurity](../../models/operations/GetTicketingConnectionIdAgentSecurity.md) | :heavy_check_mark:                                                                                                                                 | The security requirements to use for the request.                                                                                                  |


### Response

**[com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentResponse](../../models/operations/GetTicketingConnectionIdAgentResponse.md)**


## getTicketingConnectionIdAgentId

Retrieve a agent

### Example Usage

```java
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentIdRequest;
import com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentIdResponse;
import com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentIdSecurity;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            GetTicketingConnectionIdAgentIdRequest req = new GetTicketingConnectionIdAgentIdRequest("ipsa", "delectus");            

            GetTicketingConnectionIdAgentIdResponse res = sdk.agent.getTicketingConnectionIdAgentId(req, new GetTicketingConnectionIdAgentIdSecurity("tempora") {{
                jwt = "";
            }});

            if (res.ticketingAgent != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                                                              | Type                                                                                                                                                   | Required                                                                                                                                               | Description                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                              | [com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentIdRequest](../../models/operations/GetTicketingConnectionIdAgentIdRequest.md)   | :heavy_check_mark:                                                                                                                                     | The request object to use for the request.                                                                                                             |
| `security`                                                                                                                                             | [com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentIdSecurity](../../models/operations/GetTicketingConnectionIdAgentIdSecurity.md) | :heavy_check_mark:                                                                                                                                     | The security requirements to use for the request.                                                                                                      |


### Response

**[com.Unified.Unified_to.models.operations.GetTicketingConnectionIdAgentIdResponse](../../models/operations/GetTicketingConnectionIdAgentIdResponse.md)**


## getUcConnectionIdAgent

List all agents

### Example Usage

```java
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.GetUcConnectionIdAgentRequest;
import com.Unified.Unified_to.models.operations.GetUcConnectionIdAgentResponse;
import com.Unified.Unified_to.models.operations.GetUcConnectionIdAgentSecurity;
import java.time.LocalDate;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            GetUcConnectionIdAgentRequest req = new GetUcConnectionIdAgentRequest("suscipit") {{
                contactId = "molestiae";
                limit = 7917.25d;
                offset = 8121.69d;
                order = "voluptatum";
                query = "iusto";
                sort = "excepturi";
                updatedGte = LocalDate.parse("2022-01-28");
            }};            

            GetUcConnectionIdAgentResponse res = sdk.agent.getUcConnectionIdAgent(req, new GetUcConnectionIdAgentSecurity("temporibus") {{
                jwt = "";
            }});

            if (res.ucAgents != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                                            | Type                                                                                                                                 | Required                                                                                                                             | Description                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                            | [com.Unified.Unified_to.models.operations.GetUcConnectionIdAgentRequest](../../models/operations/GetUcConnectionIdAgentRequest.md)   | :heavy_check_mark:                                                                                                                   | The request object to use for the request.                                                                                           |
| `security`                                                                                                                           | [com.Unified.Unified_to.models.operations.GetUcConnectionIdAgentSecurity](../../models/operations/GetUcConnectionIdAgentSecurity.md) | :heavy_check_mark:                                                                                                                   | The security requirements to use for the request.                                                                                    |


### Response

**[com.Unified.Unified_to.models.operations.GetUcConnectionIdAgentResponse](../../models/operations/GetUcConnectionIdAgentResponse.md)**


## patchTicketingConnectionIdAgentId

Update a agent

### Example Usage

```java
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.PatchTicketingConnectionIdAgentIdRequest;
import com.Unified.Unified_to.models.operations.PatchTicketingConnectionIdAgentIdResponse;
import com.Unified.Unified_to.models.operations.PatchTicketingConnectionIdAgentIdSecurity;
import com.Unified.Unified_to.models.shared.PropertyTicketingAgentRaw;
import com.Unified.Unified_to.models.shared.TicketingAgent;
import com.Unified.Unified_to.models.shared.TicketingEmail;
import com.Unified.Unified_to.models.shared.TicketingEmailType;
import com.Unified.Unified_to.models.shared.TicketingTelephone;
import com.Unified.Unified_to.models.shared.TicketingTelephoneType;
import java.time.LocalDate;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            PatchTicketingConnectionIdAgentIdRequest req = new PatchTicketingConnectionIdAgentIdRequest("ab", "quis") {{
                ticketingAgent = new TicketingAgent(                new PropertyTicketingAgentRaw();) {{
                    createdAt = LocalDate.parse("2022-05-09");
                    emails = new com.Unified.Unified_to.models.shared.TicketingEmail[]{{
                        add(new TicketingEmail("maiores") {{
                            email = "Rita.Will87@yahoo.com";
                            type = TicketingEmailType.OTHER;
                        }}),
                    }};
                    id = "7cc78ca1-ba92-48fc-8167-42cb73920592";
                    name = "Curtis Morissette";
                    telephones = new com.Unified.Unified_to.models.shared.TicketingTelephone[]{{
                        add(new TicketingTelephone("corporis") {{
                            telephone = "fuga";
                            type = TicketingTelephoneType.OTHER;
                        }}),
                        add(new TicketingTelephone("saepe") {{
                            telephone = "iste";
                            type = TicketingTelephoneType.OTHER;
                        }}),
                        add(new TicketingTelephone("ipsa") {{
                            telephone = "quidem";
                            type = TicketingTelephoneType.WORK;
                        }}),
                        add(new TicketingTelephone("mollitia") {{
                            telephone = "reiciendis";
                            type = TicketingTelephoneType.FAX;
                        }}),
                    }};
                    updatedAt = LocalDate.parse("2022-08-29");
                }};;
            }};            

            PatchTicketingConnectionIdAgentIdResponse res = sdk.agent.patchTicketingConnectionIdAgentId(req, new PatchTicketingConnectionIdAgentIdSecurity("dolorem") {{
                jwt = "";
            }});

            if (res.ticketingAgent != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                                                                  | Type                                                                                                                                                       | Required                                                                                                                                                   | Description                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                  | [com.Unified.Unified_to.models.operations.PatchTicketingConnectionIdAgentIdRequest](../../models/operations/PatchTicketingConnectionIdAgentIdRequest.md)   | :heavy_check_mark:                                                                                                                                         | The request object to use for the request.                                                                                                                 |
| `security`                                                                                                                                                 | [com.Unified.Unified_to.models.operations.PatchTicketingConnectionIdAgentIdSecurity](../../models/operations/PatchTicketingConnectionIdAgentIdSecurity.md) | :heavy_check_mark:                                                                                                                                         | The security requirements to use for the request.                                                                                                          |


### Response

**[com.Unified.Unified_to.models.operations.PatchTicketingConnectionIdAgentIdResponse](../../models/operations/PatchTicketingConnectionIdAgentIdResponse.md)**


## postTicketingConnectionIdAgent

Create a agent

### Example Usage

```java
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.PostTicketingConnectionIdAgentRequest;
import com.Unified.Unified_to.models.operations.PostTicketingConnectionIdAgentResponse;
import com.Unified.Unified_to.models.operations.PostTicketingConnectionIdAgentSecurity;
import com.Unified.Unified_to.models.shared.PropertyTicketingAgentRaw;
import com.Unified.Unified_to.models.shared.TicketingAgent;
import com.Unified.Unified_to.models.shared.TicketingEmail;
import com.Unified.Unified_to.models.shared.TicketingEmailType;
import com.Unified.Unified_to.models.shared.TicketingTelephone;
import com.Unified.Unified_to.models.shared.TicketingTelephoneType;
import java.time.LocalDate;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            PostTicketingConnectionIdAgentRequest req = new PostTicketingConnectionIdAgentRequest("corporis") {{
                ticketingAgent = new TicketingAgent(                new PropertyTicketingAgentRaw();) {{
                    createdAt = LocalDate.parse("2022-04-01");
                    emails = new com.Unified.Unified_to.models.shared.TicketingEmail[]{{
                        add(new TicketingEmail("culpa") {{
                            email = "Franco.Hane@yahoo.com";
                            type = TicketingEmailType.HOME;
                        }}),
                        add(new TicketingEmail("consequuntur") {{
                            email = "Veronica.Brakus@hotmail.com";
                            type = TicketingEmailType.HOME;
                        }}),
                    }};
                    id = "fa946773-9251-4aa5-ac3f-5ad019da1ffe";
                    name = "Miss Irma Wolff";
                    telephones = new com.Unified.Unified_to.models.shared.TicketingTelephone[]{{
                        add(new TicketingTelephone("reprehenderit") {{
                            telephone = "perferendis";
                            type = TicketingTelephoneType.WORK;
                        }}),
                        add(new TicketingTelephone("dicta") {{
                            telephone = "ut";
                            type = TicketingTelephoneType.MOBILE;
                        }}),
                        add(new TicketingTelephone("iusto") {{
                            telephone = "corporis";
                            type = TicketingTelephoneType.HOME;
                        }}),
                    }};
                    updatedAt = LocalDate.parse("2022-04-24");
                }};;
            }};            

            PostTicketingConnectionIdAgentResponse res = sdk.agent.postTicketingConnectionIdAgent(req, new PostTicketingConnectionIdAgentSecurity("enim") {{
                jwt = "";
            }});

            if (res.ticketingAgent != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                                                            | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                            | [com.Unified.Unified_to.models.operations.PostTicketingConnectionIdAgentRequest](../../models/operations/PostTicketingConnectionIdAgentRequest.md)   | :heavy_check_mark:                                                                                                                                   | The request object to use for the request.                                                                                                           |
| `security`                                                                                                                                           | [com.Unified.Unified_to.models.operations.PostTicketingConnectionIdAgentSecurity](../../models/operations/PostTicketingConnectionIdAgentSecurity.md) | :heavy_check_mark:                                                                                                                                   | The security requirements to use for the request.                                                                                                    |


### Response

**[com.Unified.Unified_to.models.operations.PostTicketingConnectionIdAgentResponse](../../models/operations/PostTicketingConnectionIdAgentResponse.md)**


## putTicketingConnectionIdAgentId

Update a agent

### Example Usage

```java
package hello.world;

import com.Unified.Unified_to.UnifiedTo;
import com.Unified.Unified_to.models.operations.PutTicketingConnectionIdAgentIdRequest;
import com.Unified.Unified_to.models.operations.PutTicketingConnectionIdAgentIdResponse;
import com.Unified.Unified_to.models.operations.PutTicketingConnectionIdAgentIdSecurity;
import com.Unified.Unified_to.models.shared.PropertyTicketingAgentRaw;
import com.Unified.Unified_to.models.shared.TicketingAgent;
import com.Unified.Unified_to.models.shared.TicketingEmail;
import com.Unified.Unified_to.models.shared.TicketingEmailType;
import com.Unified.Unified_to.models.shared.TicketingTelephone;
import com.Unified.Unified_to.models.shared.TicketingTelephoneType;
import java.time.LocalDate;

public class Application {
    public static void main(String[] args) {
        try {
            UnifiedTo sdk = UnifiedTo.builder()
                .build();

            PutTicketingConnectionIdAgentIdRequest req = new PutTicketingConnectionIdAgentIdRequest("accusamus", "commodi") {{
                ticketingAgent = new TicketingAgent(                new PropertyTicketingAgentRaw();) {{
                    createdAt = LocalDate.parse("2022-10-22");
                    emails = new com.Unified.Unified_to.models.shared.TicketingEmail[]{{
                        add(new TicketingEmail("voluptates") {{
                            email = "Kennedi.Mante50@hotmail.com";
                            type = TicketingEmailType.HOME;
                        }}),
                    }};
                    id = "1e91e450-ad2a-4bd4-8269-802d502a94bb";
                    name = "Lucia Kemmer";
                    telephones = new com.Unified.Unified_to.models.shared.TicketingTelephone[]{{
                        add(new TicketingTelephone("necessitatibus") {{
                            telephone = "aliquid";
                            type = TicketingTelephoneType.OTHER;
                        }}),
                        add(new TicketingTelephone("dolor") {{
                            telephone = "sint";
                            type = TicketingTelephoneType.FAX;
                        }}),
                        add(new TicketingTelephone("dolorum") {{
                            telephone = "debitis";
                            type = TicketingTelephoneType.MOBILE;
                        }}),
                    }};
                    updatedAt = LocalDate.parse("2022-07-21");
                }};;
            }};            

            PutTicketingConnectionIdAgentIdResponse res = sdk.agent.putTicketingConnectionIdAgentId(req, new PutTicketingConnectionIdAgentIdSecurity("illum") {{
                jwt = "";
            }});

            if (res.ticketingAgent != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                                                              | Type                                                                                                                                                   | Required                                                                                                                                               | Description                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                              | [com.Unified.Unified_to.models.operations.PutTicketingConnectionIdAgentIdRequest](../../models/operations/PutTicketingConnectionIdAgentIdRequest.md)   | :heavy_check_mark:                                                                                                                                     | The request object to use for the request.                                                                                                             |
| `security`                                                                                                                                             | [com.Unified.Unified_to.models.operations.PutTicketingConnectionIdAgentIdSecurity](../../models/operations/PutTicketingConnectionIdAgentIdSecurity.md) | :heavy_check_mark:                                                                                                                                     | The security requirements to use for the request.                                                                                                      |


### Response

**[com.Unified.Unified_to.models.operations.PutTicketingConnectionIdAgentIdResponse](../../models/operations/PutTicketingConnectionIdAgentIdResponse.md)**
