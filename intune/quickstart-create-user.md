---
title: Quickstart - Create a user in Intune
description: Quickstart - Create a user in Intune.
services: microsoft-intune
author: ErikjeMS

ms.service: microsoft-intune
ms.topic: quickstart
ms.date: 10/30/2018
ms.author: erikje
---

# Quickstart: Create a user and assign a license to it

In this quickstart, you'll create a user and then assign a license to that user. When using Intune, each person that you want to have access to company data must have a user account. Intune admins can later configure such users to manage access control.

If you don’t have an Intune subscription, [sign up for a free trial account](free-trial-sign-up.md).

## Sign in to Intune

Sign in to the [Intune Portal](https://aka.ms/intuneportal) as a [Global administrator or an Intune Service administrator](users-add.md#types-of-administrators). If you have created an Intune Trial subscription, the account you created the subscription with is the Global administrator.

## Create a user

People must have a user account to enroll in Intune device management.

1. In Intune, choose **Users** > **All users** > **New user**.
![Browser](media/quickstart-create-user/create-user.png)
2. In the **Name** box enter a name, such as *Dewey Kellum*.
3. In the **User name** box enter a user identifier, such as Dewey@contoso.onmicrosoft.com.

    > [!NOTE]
    > If you haven't configured your customer domain name, use the verified domain name that you used to create the Intune subscription (or [free trial](free-trial-sign-up.md#sign-up-for-a-microsoft-intune-free-trial)). 

4. Choose **Show password** and make a note of the automatically generated password so that you can sign in to a test device.
5. Choose **Create**.

## Assign a license to the user

After you've created a user, you must use the [Office 365 portal](http://go.microsoft.com/fwlink/p/?LinkId=698854) to assign an Intune license to that user. Without assigning a license, they can't enroll their device into Intune. 

1. Sign in to the [Office 365 portal](http://go.microsoft.com/fwlink/p/?LinkId=698854) with the same credentials you used to sign in to Intune.
2. Choose **Users** > **Active Users** > choose the user you just created.
3. Next to **Product licenses** select **Edit**.
4. Under **Location**, choose a location for the user.
5. Click **On** next to the Intune license (or another license that you have that includes Intune). The displayed [product name](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-service-plan-reference)** is used as the service plan in the Azure management 

   > [!NOTE]
   > This setting uses one of your licenses for this user. If you are using a trial environment, you would later reassign this license to a real user in a live environment.
6. Choose **Save** > **Close**.

The new active Intune user will now show that they are using an **Intune** license.

## Clean up resources

If you don't need this user any more, you can delete the user by navigating to the [Office 365 portal](http://go.microsoft.com/fwlink/p/?LinkId=698854) and choose **Users** > **Active users** > *choose the user in the list* > **Delete user** > **Delete user** > **Confirm changes** > **Close**.

## Next steps

In this quickstart, you created a user and assigned a license to the user. You can now assign that user to a group.

> [!div class="nextstepaction"]
> [Create a group](quickstart-create-group.md)
