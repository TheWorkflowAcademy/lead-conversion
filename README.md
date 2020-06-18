# lead-conversion
Shows off Lead conversion via API in Zoho CRM — what parameters need to be passed, and how to update the resultant records.
# What do you need to execute this function?
* Make sure you've set up your Lead Conversion Mapping.
* This function relies on the "Convert Lead" API call. So you'll need an established connection between the CRM and itself with .modules.all permissions.
# Why API and Not zoho.crm.convertLead()?
zoho.crm.convertLead() is a built-in Deluge function — I honestly forget why it didn't work in this scenario, I'm sure someone smarter could have gotten it to work! If you have the wherewithal to try, by all means.
# Note on Lead Conversion Mapping
The Convert Map also contains information on the converted Deal. This can be a bit confusing — most data will pass from the Lead to the resultant records automatically, based on the info in the "Lead Conversion Mapping" settings. However, some information on the Deal (Stage, Amount, Closing Date, Pipeline, off the top of my head) needs to be stipulated WITHIN the Conversion action, i.e. they can't be set within Lead Conversion Mapping.
