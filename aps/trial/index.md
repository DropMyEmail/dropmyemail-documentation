---
layout: default
title:  "APS"
date:   2014-06-24 12:00:30
categories: aps
---

## Trying out Dropmyemail APS package

We provide a sandbox for testing our package. This sandbox allows you to try the provisioning process. There are some limitations with the sandbox. The sandbox is confined within a private virtual network. It does not have access to the public Internet. As such it cannot receive or send emails. We can only demonstrate the journal setup process.

To try our package with working Exchange email accounts, please contact our [sales team](mailto:sales@dropmyemail.com) for further instructions.

### Install VPN Client

To access the VPN, you need a VPN client. We are using the OpenVPN protocol. Please [download the certificates](https://s3-ap-southeast-1.amazonaws.com/static.documentation.dropmyemail.com/dropmyemail.vpn.zip) necessary to access the VPN. It is password protected, please approach us for the password.

If you are on Windows, please follow the instructions [here](http://doc.apsstandard.org/portal/sandbox/vpn-win/)

If you are on Mac, please follow the instructions [here](http://doc.apsstandard.org/portal/sandbox/vpn-macos/)

### Logging into the customer control panel

Please login to the panel using the following

 - url: [https://z.hexlync.apsdemo.org/single.html](https://z.hexlync.apsdemo.org/single.html)
 - login: katherine
 - password: nxcHS~-5[B

### The home screen

Upon logging in, you should be greeted with the home screen.

<img src="https://s3-ap-southeast-1.amazonaws.com/static.documentation.dropmyemail.com/pa-home-screen.png"/>

This is the first page your customer would see. The package screen could be found by clicking on __Fictional Archive__.

### The archive screen

<img src="https://s3-ap-southeast-1.amazonaws.com/static.documentation.dropmyemail.com/pa-archive-screen.png" />

We show a table of email accounts that is present in the customer's subscription. It is always kept in sync with changes in the customer's email accounts.

To add an account for archiving, select the account and click __Add__. To disable, simply select an account and click __Remove__. The setup could take about 5 minutes.

In the background, our servers will communicate with the Parallels Automation system to get information about the email accounts, such as the password and other settings. Our servers will then setup journaling on the Exchange server. Next, the archiving process will kick in and retrieve the emails onto our servers for archival. The entire process is automated. Notice all the user needs to do is to click __Add__. The status shown here depicts the progress of the journal setup(setting up journaling on Exchange). The archival process generally takes longer.

### Logging in to Dropmyemail APS admin dashboard

The Dropmyemail admin dashboard can be accessed by clicking on the __Login to Fictional Archive__ button. It automatically logs the user into Dropmyemail Archive.

<img src="https://s3-ap-southeast-1.amazonaws.com/static.documentation.dropmyemail.com/dme-aps-dashboard.png"/>

In here you will find all the features present in our Archive product, such as viewing emails, search, downloading of emails, migrate or restoring of emails. The user interface can be customized such that it becomes white labelled with your brand. You may also choose to disable specific features such as migration.

### Adding more email accounts

If you want to add more email accounts on the sandbox to see the syncing, please click on __Hosted Exchange__ entry in the dropdown found on the top right corner of the page.

<img src="https://s3-ap-southeast-1.amazonaws.com/static.documentation.dropmyemail.com/pa-subscriptions-box.png" />

You should be led to the home screen of the __Hosted Exchange__ package. Click on the __Emails__ tab and add the mailbox.

<img src="https://s3-ap-southeast-1.amazonaws.com/static.documentation.dropmyemail.com/pa-email-screen.png" />

If there are any questions, please do not hesitate to contact our [sales team](mailto:sales@dropmyemail.com).
