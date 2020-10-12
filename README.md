Description
-----------
According to https://backdropcms.org/upgrade-from-drupal/features-removed-core
the Shortcut module was removed from Backdrop core as "a feature not used by the
majority of websites". This module brings it back to Backdrop as a contributed
module.

Installation
------------
Download and place the recommended version of the module in your website's
modules directory, go to the **Functionality** page (`/admin/modules`) and
enable the **Shortcut** module.

Alternatively, just run on CLI:
```
brush -y dl shortcut
brush -y en shortcut
```

Configuration
-------------

Go to **Configuration > User interface > Shortcuts** (`admin/config/user-interface/shortcut`)
page to manage shortcut sets. You can create new shortcut sets, delete existing
ones, change set names, list links and add or delete shortcut links.

Go to **Configuration > User accounts > Permissions** (`admin/config/people/permissions#module-shortcut`)
and set desired permissions for user roles.  

Admins can can go to individual users' account pages (`user/[uid]/shortcuts`) and
assign specific shortcut sets to them.


Using
-------------

There are two ways of displaying the shortcuts:

1) Go to **Structure > Layouts > [select layout] > Manage blocks** and add the
Shortcuts block to any region (for example, to HEADER region). You can style the
Shortcut block output;

or

2) Go to **Configuration > User accounts > Permissions** (`admin/config/people/permissions#module-admin_bar`)
and give authenticated (or any other) role the `Access administration bar`
permission, clear cache and the new `My shortcuts` menu item will appear on the
admin bar.

Troubleshooting
---------------
Report all the issues on https://github.com/backdrop-contrib/shortcut/issues.

Credits
-------
The [Shortcut](https://www.drupal.org/project/protected_submissions) module had
initially been created for Drupal and has been ported to Backdrop by [AltaGrade](https://www.altagrade.com) team.
