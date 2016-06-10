---
layout: default
title:  "APS"
date:   2014-06-24 12:00:30
categories: aps
---

## Frequently Asked Questions

### Provisioning steps

Below are the steps we perform on Exchange via automated scipts.

#### Connect via WinRM

We connect to Exchange via [Windows Remote Management](http://msdn.microsoft.com/en-us/library/aa384426)

#### Create a distribution group.
A distribution group is like a mailing list. We create one to group the users whom we want to receive emails from.

#### Add the users into the distribution group
Users added to the group automatically gets his or her emails journaled.

#### Create a mailbox which will act as the journal recipient
A regular mailbox is created which will function as the journal recipient.

#### Create journal rule
Finally we create a journal rule which states that all emails sent to users belonging to the distribution group, should have their emails sent to the journal recipient.

In the case of removal, we remove all the objects created in Exchange(journal rule, mailbox and distribution group). Leaving the mailbox alone. Let me explore other use cases.

### When the user changes his password or email

For journaling even if the password changes, emails will still be sent to the journal recipient. For changes in email itself, our package registers itself to listen to changes in the account. When there are changes, PA will notify us. Our server will then query PA to get the latest changes.

### How about email aliases?

We track email aliases. They do not count to the seat, hence does not add to the pricing. Aliases will be linked to the account and shown in the interface.

### How about disk usage?

We remove the emails from the journal account once we have archived them. They do not add to the disk space on your servers.

### How to remove email from archive?

If you do not wish to keep emails archived with Dropmyemail anymore, you can remove it via Customer Controller Panel (CCP). Please note that the mailbox must remain in OSA before trying to remove it from Dropmyemail archives. Once you remove it, you loose all the archives of the email.

If you wish to continue accessing the existing email archives, we recommend you to de-activate particular email address at Dropmyemail Dashboard by selecting the particular mail box and clicking De-Activate button.

In your CCP, check the tick box of already enabled email and then click on Remove button. Removal process might take few minutes to complete.

If you have already deleted your mailbox from OSA and need to remove email from Dropmyemail archives, please contact our <a href="mailto:support@dropmyemail.com">support team</a>.