
# confluence-banner
a confluence banner with scriptrunner

### Script fragment
This is the most important thing. I made a script fragment with a condition. In the condition, I made some settings for time, group and whether this user has already read the news banner.

 - It is a web panel
 - Location: I used "atl.confluence.header"

**Properties in the Condition**
|propery|description  |
|--|--|
|pageID|On this page with this ID, I save the users, which clicked on the close button. The informations will be stored in a TextProperty on that page.|
|from / dateTo| here you can set the date in the predefined format|
|groupname|here you can define the group, which should get the message. If empty, every user gets the message|

**Provider Script**

The provider script has the banner and javascript for calling the REST Endpoint.
Also here you have to define the pageID

### REST Endpoint
The REST Endpoint saves the user which clicked the close button on the created confluence page in the TextProperty

### User Macro
The user macro reads all the users which are on this page in the TextProperty.

Some more description are found here: https://community.atlassian.com/t5/Confluence-articles/Confluence-Banner-with-ScriptRunner/ba-p/1503876
