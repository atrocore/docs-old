# Ldap authentication 

The LDAP module allows you to control AtroCore users via your own LDAP server. AtroCore always create user records, so If a new user is added via LDAP, a new record for this user will be created in AtroCore software autoamatically. For the new users a default role and a default team is assigned. Thease can still be changed via AtroCore Administration. 

Users can login via credentials, stored on the LDAP server or with their login and password.

## Administrator Functions

After the module is installed, a new LDAP panel is added in "Adminitration / Authentification". LDAP Authentification should be activated. After it you will be able to configure the connection to your LDAP Server. 

![ldap setting](_assets/Ldap/ldap_setting.png)

## Logging in by a user

To log in the user should use the Username (in blue square) and Password (in green square) stored on the LDAP Server. 

![user login menu](_assets/Ldap/user_login_menu.png)

After a User logs in for a first time a new user record for him is created in the AtroCore software (see "Administration / Users"). Default role (in green square) and Team (in blue square) are assigned to this user by default. Both can be changed by the AtroCore Administrator.

![team and role](_assets/Ldap/team_and_role.png)

![base team and role](_assets/Ldap/team_and_role_base.png)