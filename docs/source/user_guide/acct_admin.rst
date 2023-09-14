.. _acct:

Account Administration
=======================

Managing your Account
-----------------------

When your account is first activated, the default shell is set to *bash*.

The *tcsh* shell is also available. To change your shell to tcsh, add the following line:

exec -l /bin/tcsh

to the end of the file named .bash_profile , located in your home ( $HOME ) directory. 
To begin using this new shell, you can either log out and then log back in, or execute exec -l /bin/tcsh on your command line.

The Campus Cluster uses the *module* system to set up the user environment. 
See the section `Managing Your Environment (Modules) <#modules>`__ for details.

You can reset your NetID password at the `Password Management <https://identity.uillinois.edu/>`__ page.
