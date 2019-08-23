---
description: Managing rebels at the local group level.
---

# Using the Rebels Manager

Each local group has credentials to the Rebels Manager. This app allows them to manage their rebels and is frequently improved based on user feedback.

{% hint style="info" %}
**Looking for support?** **Want to suggest a feature?** Please get in touch on our Mattermost [\#rebels-manager](https://organise.earth/xrbelgium/channels/rebels-manager) channel.
{% endhint %}

## Features

* Rebels signing up on extinctionrebellion.be are added to the database
* Rebels are synced with Mailtrain, the emailing app

## Add a signup form to your local group website

Please first get in touch with it@extinctionrebellion.be and provide your website URL. We will need to allow signups from your website beforehand.

```markup
<form method="post" action="https://rebels.extinctionrebellion.be/rebels">
  <input type="text" name="rebel[name]" id="rebel_name">
  <input type="email" name="rebel[email]" id="rebel_email" required>
  <input type="tel" name="rebel[phone]" id="rebel_phone">
  <input type="text" name="rebel[postcode]" id="rebel_postcode">

  <!-- ask it@extinctionrebellion.be for your Local Group ID -->
  <input type="hidden" name="rebel[local_group_id]" id="rebel_local_group_id" value="[YOUR_LOCAL_GROUP_ID]">

  <!-- for notes/skills -->
  <textarea name="rebel[notes]" id="rebel_notes"></textarea>

  <input type="checkbox" name="rebel[consent]" id="rebel_consent">

  <!-- value can be: en, fr, nl -->
  <input type="hidden" name="rebel[language]" id="rebel_language" value="en">

  <!-- rebel will be redirected to the global 'Thank You' page -->
  <!-- but you can provide another URL -->
  <input type="hidden" name="rebel[redirect]" id="rebel_redirect" value="https://xr-city.be/welcome">

  <input type="submit" value="Join the Rebellion">
</form>
```

## Contributing

* **As a user,** we strongly suggest you to provide feedback and suggest changes/new features on the [\#rebels-manager](https://organise.earth/xrbelgium/channels/rebels-manager) Mattermost channel
* **As a developer,** feel free to browse the [Github repository](https://github.com/extinctionrebellion/RebelsManager) and get involved into the development



