---
Order: 20
xref: ccm-administration-users
Title: Users
Description: Information about configuring Users within the Chocolatey Central Management Administration section
---

In Chocolatey Central Management, Users are people who are given access to login in, and perform operations.

Users can be accessed by going to Administration on the left-hand navigation and selecting Users.

![Users menu entry on the Chocolatey Central Management Dashboard](/assets/images/ccm/users/ccm-users-menu.png)

## Creating a User

> :choco-info: **NOTE**
>
> If you do not see the **+ Create new user** button, please see your Administrator to determine if your account has the _Creating new user_ permission.

On the main Users page, select the **+ Create New User** button.

![Create New User button on the Users page](/assets/images/ccm/users/ccm-users-new.png)

You will then be presented with the `Create New User` window where you can enter all the information for the User, including `First Name`, `Email address`, etc.

![Creating New User Setting User Properties](/assets/images/ccm/users/ccm-users-set-properties.png)

Next you'll want to click over to `Roles``. This window will allow you to select what specific [Roles](xref:ccm-administration-roles) you wish to give your new User.

![Creating New User Setting Roles](/assets/images/ccm/users/ccm-users-set-roles.png)

Click :floppy_disk: **Save** to close the window and create the new User.
A green toast notification will be shown once the operation completes successfully.

## Editing a User

> :choco-info: **NOTE**
>
> If you do not see the **Edit** menu entry or the :gear: **Actions** buttons, please see your Administrator to determine if your account has the _Editing user_ permission.

On the main Users page, [find](#searching-for-a-user) the User you want to edit.
Select the :gear: **Actions** button on the left-hand side of the User, and then select **Edit** to open the _Edit User_ window.

![Edit menu entry in User actions flyout menu](/assets/images/ccm/users/ccm-users-edit.png)

From the **Edit Role** window, you can modify all the properties for a User, for example, `First Name`, `Phone number`, etc. In addition, you can alter the [Roles](xref:ccm-administration-roles) associated with the User.

Once modifications are complete, click the :floppy_disk: **Save** button.
A green toast notification will be shown once the operation completes successfully.

## Fine grained permissions

In addition to configuring a set of Roles for an individual User, so can set speicial permissions for an individual User.

On the main Users page, [find](#searching-for-a-user) the User you want to edit.
Select the :gear: **Actions** button on the left-hand side of the User, and then select **Permission** to open the _Permissions_ window.

![Permissions menu entry in User actions flyout menu](/assets/images/ccm/users/ccm-users-permissions.png)

From the tree of permissions, check/uncheck the permissions that are needed.

Once modifications are complete, click the :floppy_disk: **Save** button.
A green toast notification will be shown once the operation completes successfully.

## Deleting a User

> :choco-info: **NOTE**
>
> If you do not see the **Delete** menu entry or the :gear: **Actions** buttons, please see your Administrator to determine if your account has the _Deleting user_ permission.

On the main Users page, [find](#searching-for-a-user) the User that needs to be deleted.
Select the :gear: **Actions** button on the left-hand side of the User, and then select **Delete**.
A prompt will be shown asking `Are you sure?`.
Click `Cancel` to not continue with the operation.
Click `Yes` to proceed with the operation.
A green toast notification will be shown once the operation completes successfully.

## Unlocking a User

> :choco-info: **NOTE**
>
> If you do not see the **Unlock** menu entry or the :gear: **Actions** buttons, please see your Administrator to determine if your account has the _Editing user_ permission.

If a User enters the wrong login information 5 times, their account will become locked.
To allow them to attempt to login again, the account will need to be unlocked.
On the main Users page, [find](#searching-for-a-user) the User that is locked out.
Select the :gear: **Actions** button on the left-hand side of the User, and then select **Unlock**.
A green toast notification will be shown once the operation completes successfully.

![Action menu item showing how to unlock a User](/assets/images/ccm/users/unlock-a-user.png)

## Searching for a User

By default, there is a single search box, which can be used to search for a given User by their `User name`, `First Name`, `Surname`, and `Email`.

Clicking the `Show advanced filters` link, provide additional filtering options:

- Permissions
- Role
- Only locked users

## Exporting User Information

From the main Users page, it is possible to export all User information into either PDF or Excel format.
This can be done by using either the `Export | Export to PDF`, or the `Export | Export to Excel` button.

This will generate a file name similar to `Chocolatey_Users_20231122_130612.xlsx`, or `Chocolatey_Users_20231122_130612.pdf`.

## Pre-Configured Users

In a fresh installation of Chocolatey Central Management, there is a single pre-configured User called `ccmadmin`, which has been allocated the `CCM Admin` Role.