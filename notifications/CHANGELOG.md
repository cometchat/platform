# Notifications v1.9.6 | 2026-09-15
## New
- None

## Enhancements
- @mention notifications now work for groups having over 1000 members.

## Fixes
- None
<br/>

# Notifications v1.9.5 | 2026-09-02
## New
- Added support for subscribing to threads, allowing users to receive notifications for every reply in threads they have joined while remaining quiet in threads they have not subscribed to. The `Replies` push preference now accepts `Notify for subscribed threads`
- Added notifications when a user's message is quoted in a conversation. The `Quoted replies` push preference now accepts `Notify when my message is quoted`.

## Enhancements
- None

## Fixes
- None
<br/>

# Notifications v1.9.4 | 2026-08-06
## New
- None

## Enhancements
- Raise notification urgency for web push

## Fixes
- None
<br/>

# Notifications v1.9.3 | 2026-07-13
## New
- None

## Enhancements
- None

## Fixes
- Expired and unregistered Apple (APNs) device tokens are now automatically removed when Apple reports them as no longer valid, preventing repeated push attempts to devices that can no longer receive notifications.
<br/>

# Notifications v1.9.2 | 2026-06-29

## New
- Introduced Notification Templates for Cards, enabling customization of push and email notifications for card messages.

## Enhancements
- None

## Fixes
- None
<br/>

# Notifications v1.9.1 | 2026-06-03

## New
- None

## Enhancements
- Added a notification preference for quoted replies, giving users more control over which conversation updates trigger notifications.

## Fixes
- None
<br/>

# Notifications v1.9.0 | 2026-05-26

## New
- Support for Push notifications based Campaign messaging

## Enhancements
- None

## Fixes
- None
<br/>

# Notifications v1.7.2 | 2026-04-21

## New
- Introduced notification templates for @user mentions, enabling customization of push notifications sent to mentioned users.
- Introduced notification templates for @all mentions, enabling customization of push notifications for group mentions.

## Enhancements
- None

## Fixes
- None
<br/>

# Notifications v1.7.1 | 2026-03-24

## New
- None

## Enhancements
- Logs API now supports multi-select filtering for Provider, Trigger, Message Category, Message Type, Receiver Type, and Reason fields.

## Fixes
- Fixed an issue in the Settings API where the GET endpoint would occasionally return stale data due to a cache invalidation failure.
<br/>


# Notifications v1.7.0 | 2026-03-17

## New
- Introduced **Notification Templates for Polls**, allowing customization of notification title and body.
- Introduced **Notification Templates for Reminders**, allowing customization of notification title and body.

## Enhancements
-  None

## Fixes
- Fixed an issue where users were unable to delete default providers configured for push notifications.

# Notifications v1.6.15 | 2026-02-05

## New
- Added support for Unread Message Count in push notifications. When enabled, the user's total unread count is included in the notification payload.

## Enhancements
- None

## Fixes
- None
</br>

# Notifications v1.6.14 | 2026-01-07

## New
- None

## Enhancements
- None

## Fixes
- Fixed an issue where the **List Muted Conversations** API returned conversations whose mute duration had already expired.
</br>

# Notifications v1.6.13 | 2025-11-17

## New
- Added support for `@all` mentions in group conversations, allowing users to notify all group members, including those with muted notifications. The `@all` label is fully customizable, enabling developers to define any trigger text (e.g., `@everyone`, `@team`, `@channel`, or any custom keyword) while maintaining the same notification behavior.

## Enhancements
- None

## Fixes
- None
</br>

# Notifications v1.6.12 | 2025-09-18

## New
- None

## Enhancements
- None
 
## Fixes
- Fixed an issue where custom message email notifications were sent without validating `sendNotification` key in message payload.
- Fixed an issue where custom message SMS notifications were sent without validating `sendNotification` key in message payload.
- Fixed an issue where group reaction notifications were also sent to other group members instead of only the message sender.
</br>

# Notifications v1.6.11 | 2025-09-09

## New
- Introduced notifications for agentic messages.

## Enhancements
- None
 
## Fixes
- None
</br>

# Notifications v1.6.10 | 2025-08-26

## New
- None

## Enhancements
- Introduced options to customize email notification payloads, allowing inclusion or exclusion of the message object and metadata for greater control over notification content.
- Introduced options to customize SMS notification payloads, allowing inclusion or exclusion of the message object and metadata for greater control over notification content.
 
## Fixes
- Fixed an issue where call notifications were not received for custom providers.
</br>

# Notifications v1.6.7 | 2025-08-04

## New
- None

## Enhancements
- None
 
## Fixes
- Fixed an issue in email notifications where `Body (Fallback)` was prioritized over `Body` for custom messages in the notifications template.
</br>

# Notifications v1.6.6 | 2025-07-09

## New
- None

## Enhancements
- Added validation to ensure provider ID is valid and matches the device platform during push token registration.
 
## Fixes
- Fixed an issue where the metadata was missing from call notifications.
</br>

# Notifications v1.6.4 | 2025-06-25

## New
- None

## Enhancements
- None
 
## Fixes
- Fixed an issue where sender and receiver metadata were missing from call notifications.
- Resolved an issue where notification sounds would not play with FCM on iOS devices.
- Fixed a bug where FCM notifications on iOS did not apply the configured notification key settings.
</br>

# Notifications v1.6.3 | 2025-06-16

## New
- None

## Enhancements
- None

## Fixes
- Fixed an issue where additional data in the payload was missing from the APNS VoIP notification.
</br>

# Notifications v1.6.1 | 2025-05-22

## New
- None

## Enhancements
- None

## Fixes
- Fixed an issue where the `conversationId` was missing from the APNS payload, which occurred in version v1.6.0. This ensures proper deep linking for a notification on iOS devices.
</br>

# Notifications v1.6.0 | 2025-05-20
## New
- None

## Enhancements
- Added the ability to configure notification preferences related to calls through the Dashboard and REST API, giving more control over how call alerts are delivered.
- Introduced options to customize push notification payloads, allowing inclusion or exclusion of the message object and metadata for greater control over notification content.
- Increased the delay between SMS and email notifications to 1 minute to help prevent duplicate or closely timed alerts.

## Fixes
- Fixed an issue where pagination in the notification logs failed to work correctly, ensuring smooth navigation through log entries.
</br>

# Notifications v1.5.0 | 2025-04-24
## New
- Introduced the ability to bypass notification preferences for mentions, ensuring users always receive alerts when they are mentioned.

## Enhancements
- None

## Fixes
- None
<br/>

# Notifications v1.4.0 | 2025-04-10
## New
- Introduced **Notification Logs** feature, allowing customers to view and track notification history for easier investigation and debugging.

## Enhancements
- None.

## Fixes
- None.   
<br/>


# Notifications v1.3.0 | 2025-03-18
## New
- Custom providers for triggering Email, SMS, and Push notifications.

## Enhancements
- None.

## Fixes
- None.   
<br/>


# Notifications v1.2.4 | 2025-02-10
### New
- None

### Enhancements
- None

### Fixes
- Fixed an issue where push notifications were mistakenly sent to deactivated users for messages and events in groups.   
<br/>


# Notifications v1.2.2 | 2024-11-28
### New
- None

### Enhancements
-  None

### Fixes
- Resolved an issue where the required details, such as type, receiver's avatar URL, receiver's uid, etc. were missing in the APNs payload.
- Resolved an issue where the list of muted conversations was always returned empty.   
<br/>


# Notifications v1.2.1 | 2024-10-01
### New
- None

### Enhancements
-  Updated notification preferences for **Message Edited** and **Message Deleted** events, enabling user customisation.

### Fixes
- None
   
<br/>


# Notifications v1.2.0 | 2024-08-29
## New

-  None

## Enhancements

-  Modified the template data structure to include `uid` and `guid` for creating the Email and SMS content using templates.

## Fixes

-  None   
<br/>


# Notifications v1.1.1 | 2024-08-07
## New

-   None

## Enhancements

-   None

## Fixes

-   Fixed a bug in Push notifications where the user_blocked event was not handled properly.
-   Fixed a bug in email notifications that was forcing privacy templates for all the emails.   
<br/>


# Notifications v1.1.0 | 2024-08-07
## New

-   Added enhanced Email notifications with improved control over notifications and preferences.
-   Added enhanced SMS notifications with improved control over notifications and preferences.

## Enhancements

-   None

## Fixes

-   None   
<br/>


# Notifications v1.0.0 | 2024-08-07
## New

-   Introduced a new notifications service with enhanced push notifications for improved control over notifications and preferences.

## Enhancements

-   None

## Fixes

-   None
   
<br/>
