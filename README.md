redmine_contacts_invoice plugins depends on redmine_contacts plugin. So first need to setup redmine_contacts plugin.

1. redmine_contacts plugin setup:

-> Paste the redmine_contacts plugins in redmine plugins directory.
   Install dependent ruby gems by following command:
   
-> bundle install --without development test

-> Migrate database and copy assets by following command:

-> bundle exec rake redmine:plugins NAME=redmine_contacts RAILS_ENV=production

You now need to restart Redmine so that it shows the newly installed plugin in the list of installed plugins ("Administration -> Plugins").

-> Go to "Administration -> Contacts" and setup plugin global settings.


2. redmine_contacts_invoice plugin setup:

-> Paste the redmine_contacts_invoice plugin in redmine plugins directory.
   Install dependent ruby gems by following command:

-> bundle install --without development test

-> Migrate database and copy assets by following command:

-> bundle exec rake redmine:plugins NAME=redmine_contacts_invoices RAILS_ENV=production

You now need to restart Redmine so that it shows the newly installed plugin in the list of installed plugins ("Administration -> Plugins").

-> Go to "Administration -> Invoices" and setup plugin global settings.

For More information visit the following link:

http://redminecrm.com/projects/invoices/pages/2
