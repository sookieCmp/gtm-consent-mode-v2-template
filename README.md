# Sookie CMP – Consent Mode v2 Template (GTM)

## Overview
This template integrates Sookie CMP with Google Tag Manager and enables Google Consent Mode v2.

It automatically:
- Sets default consent states
- Loads Sookie CMP script
- Passes configuration via global window object

## Features
- Full Consent Mode v2 support
- Secure script injection from Sookie CMP
- Lightweight implementation
- Easy setup using Sookie ID

## Configuration

### Required Field
- **Sookie ID**: Your unique CMP ID from Sookie dashboard

## How It Works
1. Default consent is set to denied (except security_storage)
2. Configuration is exposed via `window.SCOOKIE_CONFIG`
3. CMP script is loaded from:3. CMP script is loaded from:

https://app.sookie.eu/api/cookie-consent

4. Consent updates are handled by the CMP

## Permissions Used

- **inject_script**  
Loads Sookie CMP script

- **set_default_consent_state**  
Sets initial consent values

- **access_globals (write)**  
Writes configuration to `window.SCOOKIE_CONFIG`

## Security Notes
- Only loads script from official Sookie domain
- No user data is collected directly in template
- Fully compliant with Consent Mode v2 requirements

## Author
Sookie CMP

## Support
support@sookie.eu
