Instructions for Recon-NG v4.8.3:



API Keys:

   1.  **bing_api** _(optional $$$)_ - Sign up [here](http://datamarket.azure.com/dataset/bing/search) (I chose the free plan), agree to all the terms until you get to "Thank You", then go [here](https://datamarket.azure.com/account/keys) to view the key. (free account: 5000 transactions per month)

   2. **builtwith_api** - Go [here](https://api.builtwith.com/) and sign up.  Once you enter an email and password, it will show you the API key

   3. **censysio_id** - Go [here](https://censys.io/register) and sign up. Once you register, confirm your account by clicking on the link in the email. Then login and go [here](https://censys.io/account) to view the "ID" and "Secret"

   4. **censysio_secret** - Look at #3

   5. **facebook_api** - This one is a bit more in-depth.  Click [here](https://developers.facebook.com/), login to Facebook (or register if you don't have one).  Once logged in, in the top-right, click "My Apps", then "Add a new app". Click the "Add a new app" green button.  Type any name you want and select any category.  This will create a new app, now click "Dashboard" in the top left.  Copy the "App ID" and "App Secret" from that page. For this field, you want to use "App ID"

   6. **facebook_password** - _Note: Due to order of the API keys, this does not have to do with #5 above!_ This is simply your facebook password.  Or make a new facebook and use that password!

   7. **facebook_secret** - This is the "App Secret" from #5

   8. **facebook_username** - This is your facebook username that has the password listed in #6.  Make a new facebook account if you want

   9. **flickr_api** - Go [here](https://www.flickr.com/services/apps/create/) and click "Request an API Key" under "Get your API key".  Login to Yahoo (or make an account).  If you had to create a Yahoo/Flickr account, you may need to [click the link again](https://www.flickr.com/services/apps/create/) after registering.  Choose "Apply for non-commercial key".  Fill in some filler information (it really doesn't matter what you put here).  Then you will get an "API Key" and "Secret".  Use "API Key" for this entry (_Note: Untested, don't know if you need "Secret" too or what. Open bug report [here](https://bitbucket.org/LaNMaSteR53/recon-ng/issues/189/flickr-api-key-option))_

   10. **fullcontact_api** _(optional $$$)_- Go [here](https://www.fullcontact.com/developer/) and click "Get a key". Sign up.  You will be shown an API key immediately after signing up (free account: 500 Person and Company matches per month, and 60 queries per minute)

   11. **github_api** - Go [here](https://github.com/settings/tokens) (login if necessary, then click the link). Click "Generate new token" in the top right corner.  You don't need to give the token any permissions (and I recommend that you don't), just click "Generate Token".  You will be shown the token

   12. **google_api** _(optional $$$)_ - Go [here](https://console.developers.google.com/apis/library) (login if necessary). At the top left, click the dropdown "Project", then "Create project". Enter a project name, then hit "Create". Once the project is created, go [here](https://console.developers.google.com/apis/credentials) and click "Create Credentials" and select "API Keys". It displays the key to use here.  Click "close" after you save it, _not "Restrict Key"._Then go to"Library" on the left, click "Custom Search API" (bottom-ish), and click "Enable". Done! (free account: 100 search queries per day for free)

   13. **google_cse** - Go [here](https://cse.google.com/cse/all) (login if necessary).  Click "Create", enter "www.google.com" with "Sites to search", then click "Create" button.  On the next page, click "Control Panel".  Under "Sites to search", choose "Search the entire web but emphasize included sites" in the dropdown, then click the "Update" button at the bottom.  On the same page, scroll up and click "Search Engine ID" under "Details".  Thats the key to use here!

   14. **hashes_api** - Register [here](https://hashes.org/register_form.php) (or login).  Confirm your account via email link. Login with your new account, then click [here](https://hashes.org/settings.php). Your API key should be listed.

   15. **instagram_api** - Register [here](https://www.instagram.com/accounts/login/?next=%2Fdeveloper%2Fregister%2F) (or login). Once logged in, click [here](http://instagram.com/developer/clients/register/) and create a new application. Add "http://localhost:31337" as the "OAuth redirect_uri". Click "Manage Clients" at the top of the screen and the API key will be available as the "CLIENT_ID" _(Note: Instagram wasn't functioning when I wrote this...it may be different)_

   16. **instagram_secret** - Same as #15 but its "CLIENT_SECRET"

   17. **ipinfodb_api** - Register [here](http://www.ipinfodb.com/register.php). You must enter the IP you will use recon-ng from under "Server IP".  I recommend you use a VPN or server or something so the IP never changes.  Activate the account via email link.  The api key will be given to you on account activation

   18. **jigsaw_api** _(Requires $$$)_ - Register [here](https://connect.data.com/registration/signup).  Once registered, you must send a special request to get an API key.  No specifics here because its very _expensive!_.

   19. **jigsaw_password** _(Requires $$$)_ - Register [here](https://connect.data.com/registration/signup).  This is the password for your account that you create and sign up for a plan with!

   20. **jigsaw_username** _(Requires $$$)_ - Same as #19, but this is the account password.

   21. **linkedin_api** - Go [here](https://www.linkedin.com/secure/developer) (register/login if necessary) and click "Create Application". Fill out the information with random stuff...annoyingly it requires an image with the same width and height.  I used [this](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0d/Ski_trail_rating_symbol-blue_square.svg/600px-Ski_trail_rating_symbol-blue_square.svg.png). It will show you the "Client ID", which is this key. Add "http://localhost:31337" under "OAuth 2.0".  Check all the boxes under "Default Application Permissions".  Click "Update". _For this API to function fully, you must submit [this form](https://www.linkedin.com/help/linkedin/ask/API-DVR)_. Fill out information explaining what you will use it for, etc.  Pain in the butt, but necessary.

   22. **linkedin_secret** - Same as #21, but its the "Client Secret"

   23. **pwnedlist_api** - Service has been officially shut down

   24. **pwnedlist_iv** - Service has been officially shut down

   25. **pwnedlist_secret** - Service has been officially shut down

   26. **shodan_api** _(optional $$$)_- Login or register [here](https://account.shodan.io/login).  Activate your account via email.  The API key will be shown upon login. (free account: basic search capabilities. Premium account with full access is a one-time payment of $50 and pretty worth it)

   27. **twitter_api** - Go [here](https://apps.twitter.com/) and login/register as needed. Click "Create New App".  Enter in filler information of your app.  Once the application is created, click on "manage keys and access tokens".  The key is "Consumer Key (API Key)".

   28. **twitter_secret** - Same as #27, but the key is "Consumer Secret (API Secret)"

   29. **virustotal_api** _(If using a branch with it)_ - Go [here](https://www.virustotal.com/) and click "Join our community" in the top right.  Active the account via email, then login.  Click your username in the top right, then click "My API Key". The API key will be shown. A "public" API will be sufficient.


