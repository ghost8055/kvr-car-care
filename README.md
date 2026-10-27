# KVR Car Care

Installable web app for the KVR Car Care workshop and customer portal.

## Separate app entry points

- **Customer app:** open `customer.html` (or `index.html?app=customer`).
- **Owner app:** open `owner.html` (or `index.html?app=owner`).

On GitHub Pages, these are available under the repository's published URL as `/customer.html` and `/owner.html`. Install each entry from its own app page to get separate home-screen shortcuts and app names.

The customer portal contains the KVR signboard/workshop banner, vehicle and request tools, progress photos, service history, WhatsApp contact, and directions. The owner portal includes job updates, charges, invoices, and workshop history.

## GitHub Pages

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and `/ (root)`, then save.
4. Open the published HTTPS address on your phone.

## Install on a phone

- **Android:** Open the published address in Chrome and select **Install app** or **Add to Home screen**.
- **iPhone:** Open the published address in Safari, tap **Share**, then **Add to Home Screen**.

The app shell is cached for offline use after its first successful load.

## Demo sign-in and limitations

This is a static front-end demo. Customer sign-in uses a name and phone number; owner demo sign-in accepts `7093441878` or `7036705454`. There is no SMS OTP, so phone numbers are not verified and this is not secure authentication. Customer, vehicle, and service data is saved only in the current browser's local storage and does not sync between devices.

Completing a job creates an invoice in the app and opens a prefilled WhatsApp message to the customer's number. The user must review and press **Send** in WhatsApp; the app does not automatically deliver messages or attach a PDF. Use the invoice preview's print dialog to save a PDF.

Do not enter real customer information or use this demo as a secure production system. A secured backend, identity verification, shared database, and access controls are required for production use.
