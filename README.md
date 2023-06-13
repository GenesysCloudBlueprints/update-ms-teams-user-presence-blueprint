# (DRAFT) Update the presence of a Microsoft Teams user based upon a Genesys Cloud user presence update

This Genesys Cloud Developer Blueprint explains how to set up Genesys Cloud and Microsoft Azure Active Directory to update a Genesys Cloud user's presence in Microsoft Teams when a user presence change occurs in Genesys Cloud.

When an Architect workflow receives an inbound user presence change, a Microsoft Graph API call is sent to the Microsoft Teams user that is associated with the Genesys Cloud user. The Microsoft Teams user's presence is set to the MS Teams presence value that corresponds to the GC User presence value sent to the Architect workflow.

![Microsoft Teams agent view](blueprint/images/msteams-presence-workflow.png "Microsoft Teams presence update from an agent's point of view")

The following shows the end-to-end agent experience that this solution enables.

![End-to-end agent experience](blueprint/images/GCtoMSTeamsPresenceUpdatesbasedonGCPresenceChanges.gif "End-to-end agent experience")

To trigger Microsoft Teams presence updates from Genesys Cloud, you use several public APIs that are available from Genesys Cloud and Microsoft Graph. The following illustration shows the API calls between Genesys Cloud and Microsoft 365.

![The API calls between Genesys Cloud and Microsoft 365](blueprint/images/microsoft-teams-architect.png "The API calls between Genesys Cloud and Microsoft 365")
