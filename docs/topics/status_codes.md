# Status Codes

## Server

Events over the Geometry Dash servers usually send an error code denoting that the server either had an error, or you sent an invalid request.

#### Server Status Codes

| Code |                Name                                              |                                   Description                                       |
|------|------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| -1   | Invalid Request                                                  | A parameter in your [HTTP request](/endpoints/request.md) to the server was invalid.|
| -2   | [Common](/topics/status_codes?id=endpoint-specific-status-codes) | This status code is commonly used in multiple endpoints either for `taken` things, or theres none of something. |

#### Endpoint-specific Status Codes

These are Status Codes that are used in more than one place.

| Code |       Name           |           Endpoint             |               Description                |
|------|----------------------|--------------------------------|------------------------------------------|
| -2   | Taken Username       | registerGJAccount.php          | The username provided has been taken     |
| -4   | Request is too large | Account saving (69.164.210.48) | Your request to the server was too large |
| -5   | Bad login info       | Account saving (69.164.210.48) | Invalid login info was provided          |
| -6   | Something went wrong | Account saving (69.164.210.48) | Something went wrong on the servers' end |
