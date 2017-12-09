---
section: libraries
title: Migrating AngularJS Applications to from Lock v10 to Lock v11
description: How to migrate AngularJS Applications from Lock v10 to v11
toc: true
---

# Migrating AngularJS applications from Lock.js v10 to v11

## Migration Steps

<%= include('../../_includes/_get_lock_latest_version') %>

### Update angular-lock

AngularJS (a.k.a. Angular 1.x) applications usually use the [angular-lock package](https://www.npmjs.com/package/angular-lock). To use Auth0.js v9 you need to update to the latest version (3.x).

You can update the angular-lock library using npm or yarn.

```bash
# installation with npm
npm install --save angular-lock
 
# installation with yarn
yarn add angular-lock
```

The script files need to be added to your build system, or added to the project with a script tag.

```html
<script src="node_modules/angular-lock/dist/angular-lock.js"></script>
```
## Migration Steps

<%= include('../../_includes/_configure_embedded_login') %>
<%= include('../../_includes/_change_get_profile') %>
<%= include('../../_includes/_oidc_conformant') %>

## Behavioral Changes in Lock.js v11

<%= include('../../_includes/_hosted_pages') %>
<%= include('../../_includes/_popup_mode') %>

<%= include('../../_includes/_last_logged_in_window') %>
<%= include('../../_includes/_ip_ranges') %>
<%= include('../../_includes/_default_values_lock') %>
