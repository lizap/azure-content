
<properties 
    pageTitle="Supported user identities"
    description="" 
    services="remoteapp" 
    solutions="" documentationCenter="" 
    authors="ericorman" 
    manager="mbaldwin" />

<tags 
    ms.service="remoteapp" 
    ms.workload="compute" 
    ms.tgt_pltfrm="na" 
    ms.devlang="na" 
    ms.topic="article" 
    ms.date="02/20/2015" 
    ms.author="mbaldwin" />



# Supported user identities

Azure RemoteApp has two deployment methods: cloud and hybrid. Each supports using different user identities for user access to applications.  

For a hybrid collection of RemoteApp, you need to set up an Active Directory domain infrastructure on premises and an Azure Active Directory tenant with Directory Integration (and optionally single sign-on). Additionally, you need to create some Active Directory objects in the on-premises directory.  

For a cloud collection of RemoteApp, any user that has Azure Active Directory support identities can be granted user access to RemoteApp to include Microsoft Accounts.  See table below. 

Office 365 users are Azure Active Directory users. If they have Azure Active Directory hybrid, Directory synchronized accounts, they can be granted user access in a RemoteApp hybrid deployment.   

|User accounts |Cloud	|Hybrid|
|--------------|--------|------|
|:Microsoft Account| 	Yes|	No|
|:Azure Active Directory (Azure AD)|	| |	
|*Azure AD cloud only 	:|Yes	|No	|
|ADsync with password sync	:|Yes	|Yes	|
|ADsync without password sync:|	Yes	|No	|
|ADsync with AD FS	:|Yes	|Yes	|
|3rd-party Azure supported identity providers  (example Ping)	:|Yes	|No|	
|:Multi-Factor Authentication	|Yes	|Yes	|

Check out [more information](..\remoteapp-ad) about configuring Active Directory for RemoteApp.