OemproConnect is a PHP wrapper class to connect to Octeth Oempro 4.0.`*` API.

Current (v1.0) API commands supported:
  * User.Login (of course ;-)
  * Campaign.Create
  * Campaign.Update
  * Campaigns.Get
  * List.Create
  * Lists.Get
  * Subscriber.Subscribe
  * Subscribers.Get
  * Subscribers.Delete
  * Email.Create
  * Email.Update
  * Emails.Get
  * Email.EmailPreview

By now the OemproConnect only accepts JSON as responses from API, in the near future will be implemented XML responses and more methods.

Example:
```
require("OemproConnect.class.php");
$oempro = new OemproConnect();
$oempro->setApiURL("http://www.yourdomain.com/api.php");
$oempro->userLogin("userlogin", "userpassword123");

// call the methods you need
$arrCampaigns = $oempro->getCampaigns();
...
```