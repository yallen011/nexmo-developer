---
title: Send a Message Template (MTM)
meta_title: Send a WhatsApp Message Template (MTM) using the Messages API
navigation_weight: 1
---

# Send a WhatsApp Message Template (MTM)

In this code snippet you learn how to send a WhatsApp Message Template Message (MTM) using the Messages API.

> **IMPORTANT:** If a customer messages you, you have 24 hours to respond to the customer with a free-form message. After this period you must use a message template (MTM). If a customer has not messaged you first, then the first time you send a message to a user, WhatsApp requires that the message contains a template. This is explained in more detail in the [Understanding WhatsApp topic](/messages/concepts/whatsapp).

## Example

Ensure the following variables are set to your required values using any convenient method:

Key | Description
-- | --
`WHATSAPP_NUMBER` | The WhatsApp number that has been allocated to you by Nexmo.
`TO_NUMBER` | The phone number you are sending the message to.
`WHATSAPP_TEMPLATE_NAMESPACE` | The namespace ID found in your WhatsApp Business Account. Only templates created in your own namespace will work. Using an template with a namespace outside of your own results in an error code 1022 being returned.
`WHATSAPP_TEMPLATE_NAME` | The name of the template created in your WhatsApp Business Account.

> **NOTE:** Don't use a leading `+` or `00` when entering a phone number, start with the country code, for example, 447700900000.

```code_snippets
source: '_examples/messages/whatsapp/send-mtm'
application:
  type: messages
  name: 'Send a WhatsApp template'
```

## Try it out

When you run the code a WhatsApp message template (MTM) is sent to the destination number.

## Further information

* [WhatsApp documentation for Message Templates](https://developers.facebook.com/docs/whatsapp/api/messages/message-templates)
