---
layout: default
title:  "APS"
date:   2014-04-26 12:00:30
categories: aps
---

## Parallels APS

Dropmyemail provides a package to be installed on Parallels Automation. Currently we only support APS v2.0. We will show you the steps to install a white labelled package. For the purpose of this document, we will use a psuedo name called __Critical Email__ for the white label partner. Do replace the name with your company's name when applicable.

### Pre-requisites

Please obtain the package from us. We will also provide you with the authentication token for the package.

### Installation of the package on PA

The following instructions assumes you are the admin on the PA. First log in as admin.

- Click on __Applications__.
- On the __Applications__ page, click on __Import Package__. Select the local file option, and select the Dropmyemail APS package from your local drive.
- Click __Submit__

### Connecting Dropmyemail to PA

Now we need to hook up the Dropmyemail API server to the PA.

- On the __Applications__ page, click on the package __Dropmyemail__
- On the __Dropmyemail__ package page, click on the __Instances__ tab
- On the __Instances__ tab, click on __Install__
- For the __Application API end-point URI__ field, enter _http://api.staging-dropmyemail.com/v1/aps_
- For the next form, enter a name that identifies the partner for the __Name__ field. _Eg. Critical Email_
- For the __Authentication Token__ field, enter the token provided by Dropmyemail.
- Click __Finish__

### Defining the service

First we need to define the resources which we are selling. Then we need to define the service templates which sets the limit for the resources.

- Click on __Resources__
- Click on __Add New Resource Type__
- Click on __Application Service Reference__.
- Enter __Dromyemail Archive__ for the __Name__ field and click __Next__
- Select __Dropmyemail__
- You should see a series of screens with links. There should be only one link on each screen. Click on the links.

There are 3 resources. Repeat the same steps with the following input.

- Dropmyemail Archiving: Application Service Reference
- Dropmyemail Customers: Application Service, automatic provisioning
- Dropmyemail Seats: Application Service, no automatic provisioning

Once done, we need to create the service template. The following is an example of an unlimited plan.

- Click on __Service Templates__
- Click on __Add New Service Template__
- Enter __Critical Email__ for the name field. This field will appear on the customer's subscription. It should be the name of your service. Also enable the __Autoprovisioning__ checkbox. Use the default value __Custom__ for the __Type__ field. You may type anything for the __Description__ field.
- Find the earlier 3 resources we've defined, check them and click __Next__
- Adjust the limit as you need and click __Next__
- Click __Finish__

The service template is not active yet. You need to click on the template and click on __Activate__ to enable it.
