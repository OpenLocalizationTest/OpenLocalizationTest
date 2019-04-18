<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-manage-access-tokens.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b45279d64b5f9dd0766044f171fef45383be021598.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5279d64b5f9dd0766044f171fef45383be021598</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\how-to-manage-access-tokens.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing access tokens, bearer tokens, access_token, refresh_token - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Token Management for API Requests with Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Manage access tokens for API requests</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server, Microsoft R Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Machine Learning Server, formerly known as Microsoft R Server, uses tokens to identify and authenticate the user who is sending the API call within your application.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Users must authenticate when making an API call.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>They can do so with the 'POST /login HTTP/1.1' API call, after which Machine Learning Server issues a bearer token to your application for this user.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Alternately, if the organization is using Azure Active Directory (AAD), users  receive a bearer token from AAD when they authenticate.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This bearer token is a lightweight security token that grants the “bearer” access to a protected resource, in this case, Machine Learning Server's core APIs for operationalizing analytics.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>After a user has been authenticated, the application must validate the user’s bearer token to ensure that authentication was successful.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For proper access token signing and verification across your configuration, ensure that the JWT settings are exactly the same for every web node.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>These JWT settings are defined on each web node in the configuration file, appsetting.json.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Check with your administrator.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](configure-authentication.md#ldap-jwt)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Security Concerns</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Despite the fact that a party must first authenticate to receive the token, tokens can be intercepted  by an unintended party if the token is not secured in transmission and storage.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>While some security tokens have a built-in mechanism to protect against unauthorized parties, these tokens do not and must be <bpt id="p1">[</bpt>transported in a secure channel such as transport layer security (HTTPS)<ept id="p1">](configure-https.md)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If a token is transmitted in the clear, a man-in the middle attack can be used by a malicious party to acquire the token to make an unauthorized access to a protected resource.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The same security principles apply when storing or caching tokens for later use.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Always ensure that your application transmits and stores tokens in a secure manner.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>You can <bpt id="p1">[</bpt>revoke a token<ept id="p1">](#revoke)</ept> if a user is no longer permitted to make requests on the API or if the token has been compromised.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Create tokens</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The API bearer token's properties include an access_token / refresh_token pair and expiration dates.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Tokens can be generated in one of two ways:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If Active Directory LDAP or a local administrator account is enabled, then send a 'POST /login HTTP/1.1' API request to retrieve the bearer token.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If Azure Active Directory (AAD) is enabled, then <bpt id="p1">[</bpt>the token comes from AAD<ept id="p1">](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-authentication-scenarios)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more about these authentication methods.<ept id="p1">](configure-authentication.md)</ept></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Example: Token creation request</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Request<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Response<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Token Lifecycle</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The bearer token is made of an access_token property and  a refresh_token property.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The "access_token" Lifecycle</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The "refresh_token" Lifecycle</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Gets<ph id="ph1">&lt;br/&gt;</ph>Created<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Whenever the user logs in, or</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>a refreshToken api is called</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Whenever the user logs in</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Expires<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>After 1 hour (3660 seconds) of inactivity</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>After 336 hours (14 days) of inactivity</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Becomes<ph id="ph1">&lt;br/&gt;</ph>Invalid<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If the refresh_token was revoked, or</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If not used for 336 hours (14 days), or</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>When a new pair of access_token/refresh_token has been created</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If not used for 336 hours (14 days), or</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>When the refresh_token expires, or</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>When a new access_token/refresh_token pair was created, or</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If the refresh_token was revoked</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Use tokens</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>As defined by HTTP/1.1 [RFC2617], the application should send the access_token directly in the Authorization request header.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>You can do so by including the bearer token's access_token value in the HTTP request body as 'Authorization: Bearer {access_token_value}'.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>When the API call is sent with the token, Machine Learning Server attempts to validate that the user is successfully authenticated and that the token itself is not expired.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If an authenticated user has a bearer token's access_token or refresh_token that is expired, then a '401 - Unauthorized (invalid or expired refresh token)' error is returned.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If the user is not successfully authenticated, a '401 - Unauthorized (invalid credentials)' error is returned.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Example HTTP header for session creation:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Example HTTP header for publishing web service:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Renew tokens</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>A valid bearer token (with active access_token or refresh_token properties) keeps the user's authentication alive without requiring him or her to re-enter their credentials frequently.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The access_token can be used for as long as it’s active, which is up to one hour after login or renewal.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The refresh_token is active for 336 hours (14 days).</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>After the access_token expires, an active refresh_token can be used to get a new access_token / refresh_token pair as shown in the following example.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>This cycle can continue for up to 90 days after which the user must log in again.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If the refresh_token expires, the tokens cannot be renewed and the user must log in again.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>To refresh a token, use <bpt id="p1">[</bpt>the 'POST /login/refreshToken HTTP/1.1' API call<ept id="p1">](https://microsoft.github.io/deployr-api-docs/?tags=User#refresh-user-access-token)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Example: Refresh access_token</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Example request:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Example response:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Revoke refresh tokens</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>A refresh_token should be revoked:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If a user is no longer permitted to make requests on the API, or</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If the access_token or refresh_token have been compromised.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>the 'DELETE /login/refreshToken?refreshToken={refresh_token_value} HTTP/1.1' API call<ept id="p1">](https://microsoft.github.io/deployr-api-docs/?tags=User#delete-user-access-token)</ept>  to revoke a token.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Example: Revoke token</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Example request:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Example response:</source>
        </trans-unit></group></body></file></xliff>