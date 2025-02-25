---
title: 'Tutorial: Azure AD SSO integration with Yonyx Interactive Guides'
description: Learn how to configure single sign-on between Azure Active Directory and Yonyx Interactive Guides.
services: active-directory
author: jeevansd
manager: CelesteDG
ms.reviewer: celested
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.topic: tutorial
ms.date: 11/21/2022
ms.author: jeedes
---
# Tutorial: Azure AD SSO integration with Yonyx Interactive Guides

In this tutorial, you'll learn how to integrate Yonyx Interactive Guides with Azure Active Directory (Azure AD). When you integrate Yonyx Interactive Guides with Azure AD, you can:

* Control in Azure AD who has access to Yonyx Interactive Guides.
* Enable your users to be automatically signed-in to Yonyx Interactive Guides with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

## Prerequisites

To get started, you need the following items:

* An Azure AD subscription. If you don't have a subscription, you can get a [free account](https://azure.microsoft.com/free/).
* Yonyx Interactive Guides single sign-on (SSO) enabled subscription.

## Scenario description

In this tutorial, you configure and test Azure AD SSO in a test environment.

* Yonyx Interactive Guides supports **SP** initiated SSO.

* Yonyx Interactive Guides supports **Just In Time** user provisioning.

## Add Yonyx Interactive Guides from the gallery

To configure the integration of Yonyx Interactive Guides into Azure AD, you need to add Yonyx Interactive Guides from the gallery to your list of managed SaaS apps.

1. Sign in to the Azure portal using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **Yonyx Interactive Guides** in the search box.
1. Select **Yonyx Interactive Guides** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.

 Alternatively, you can also use the [Enterprise App Configuration Wizard](https://portal.office.com/AdminPortal/home?Q=Docs#/azureadappintegration). In this wizard, you can add an application to your tenant, add users/groups to the app, assign roles, as well as walk through the SSO configuration as well. [Learn more about Microsoft 365 wizards.](/microsoft-365/admin/misc/azure-ad-setup-guides)


## Configure and test Azure AD SSO for Yonyx Interactive Guides

Configure and test Azure AD SSO with Yonyx Interactive Guides using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in Yonyx Interactive Guides.

To configure and test Azure AD SSO with Yonyx Interactive Guides, perform the following steps:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
    1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with B.Simon.
    1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable B.Simon to use Azure AD single sign-on.
1. **[Configure Yonyx Interactive Guides SSO](#configure-yonyx-interactive-guides-sso)** - to configure the single sign-on settings on application side.
    1. **[Create Yonyx Interactive Guides test user](#create-yonyx-interactive-guides-test-user)** - to have a counterpart of B.Simon in Yonyx Interactive Guides that is linked to the Azure AD representation of user.
1. **[Test SSO](#test-sso)** - to verify whether the configuration works.

## Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the Azure portal, on the **Yonyx Interactive Guides** application integration page, find the **Manage** section and select **single sign-on**.
1. On the **Select a single sign-on method** page, select **SAML**.
1. On the **Set up single sign-on with SAML** page, click the pencil icon for **Basic SAML Configuration** to edit the settings.

   ![Screenshot for Edit Basic SAML Configuration.](common/edit-urls.png)

1. On the **Basic SAML Configuration** section, enter the values for the following fields:

	a. In the **Sign on URL** text box, type a URL using the following pattern:
    `https://<company name>.yonyx.com/y/conversation/?id=<guid number>`

    b. In the **Identifier (Entity ID)** text box, type a URL using the following pattern:
    `https://<company name>.yonyx.com`

	> [!NOTE]
	> These values are not real. Update these values with the actual Sign on URL and Identifier. Contact [Yonyx Interactive Guides Client support team](mailto:support@yonyx.com) to get these values. You can also refer to the patterns shown in the **Basic SAML Configuration** section in the Azure portal.

5. On the **Set up Single Sign-On with SAML** page, in the **SAML Signing Certificate** section, click **Download** to download the **Certificate (Base64)** from the given options as per your requirement and save it on your computer.

	![Screenshot for The Certificate download link.](common/certificatebase64.png)

6. On the **Set up Yonyx Interactive Guides** section, copy the appropriate URL(s) as per your requirement.

	![Screenshot for Copy configuration URLs.](common/copy-configuration-urls.png)

### Create an Azure AD test user

In this section, you'll create a test user in the Azure portal called B.Simon.

1. From the left pane in the Azure portal, select **Azure Active Directory**, select **Users**, and then select **All users**.
1. Select **New user** at the top of the screen.
1. In the **User** properties, follow these steps:
   1. In the **Name** field, enter `B.Simon`.  
   1. In the **User name** field, enter the username@companydomain.extension. For example, `B.Simon@contoso.com`.
   1. Select the **Show password** check box, and then write down the value that's displayed in the **Password** box.
   1. Click **Create**.

### Assign the Azure AD test user

In this section, you'll enable B.Simon to use Azure single sign-on by granting access to Yonyx Interactive Guides.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **Yonyx Interactive Guides**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.
1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.
1. In the **Users and groups** dialog, select **B.Simon** from the Users list, then click the **Select** button at the bottom of the screen.
1. If you are expecting a role to be assigned to the users, you can select it from the **Select a role** dropdown. If no role has been set up for this app, you see "Default Access" role selected.
1. In the **Add Assignment** dialog, click the **Assign** button.

## Configure Yonyx Interactive Guides SSO

To configure single sign-on on **Yonyx Interactive Guides** side, you need to send the downloaded **Certificate (Base64)** and appropriate copied URLs from Azure portal to [Yonyx Interactive Guides support team](mailto:support@yonyx.com). They set this setting to have the SAML SSO connection set properly on both sides.

### Create Yonyx Interactive Guides test user

In this section, a user called Britta Simon is created in Yonyx Interactive Guides. Yonyx Interactive Guides supports just-in-time user provisioning, which is enabled by default. There is no action item for you in this section. If a user doesn't already exist in Yonyx Interactive Guides, a new one is created after authentication.

> [!NOTE]
> If you need to create a user manually, you need to contact the [Yonyx Interactive Guides support team](mailto:support@yonyx.com).

## Test SSO

In this section, you test your Azure AD single sign-on configuration with following options. 

* Click on **Test this application** in Azure portal. This will redirect to Yonyx Interactive Guides Sign-on URL where you can initiate the login flow. 

* Go to Yonyx Interactive Guides Sign-on URL directly and initiate the login flow from there.

* You can use Microsoft My Apps. When you click the Yonyx Interactive Guides tile in the My Apps, this will redirect to Yonyx Interactive Guides Sign-on URL. For more information about the My Apps, see [Introduction to the My Apps](https://support.microsoft.com/account-billing/sign-in-and-start-apps-from-the-my-apps-portal-2f3b1bae-0e5a-4a86-a33e-876fbd2a4510).

## Next steps

Once you configure Yonyx Interactive Guides you can enforce session control, which protects exfiltration and infiltration of your organization’s sensitive data in real time. Session control extends from Conditional Access. [Learn how to enforce session control with Microsoft Defender for Cloud Apps](/cloud-app-security/proxy-deployment-aad).