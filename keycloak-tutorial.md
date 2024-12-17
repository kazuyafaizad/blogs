1) Toggle Client authetication in Capability Config and tick Service accounts Role, the account must be openID connect
2) Grant manage-users,view-users,query-users in Service accounts roles tab

{host}/realms/{realm}/protocol/openid-connect/token

client_id:admin-rest-client
client_secret:***** (Get from Crendetial Tab)
grant_type:client_credentials

get access token bearer

{host}/admin/realms/staging/users

format 
{
                 "username": "' . $cell2 . '",
                 "email": "' . $cell2 . '",
                 "enabled": true,
                 "firstName": "' . $cell1 . '",
                 "lastName": "",
                 "credentials": [
                     {
                     "type": "password",
                     "value": "password",
                     "temporary": false
                     }
                 ]
                 }
                 
