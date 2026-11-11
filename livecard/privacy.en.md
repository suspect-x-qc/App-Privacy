# LiveCard Privacy Policy

> Draft for review. Not yet effective. Complete the bracketed fields and confirm that the released app and its App Store privacy disclosures match this policy before publication.

Effective date: [To be provided]

Developer / responsible party: James Kou

Privacy contact: suspectx01@gmail.com

## 1. Scope

This policy explains how LiveCard handles information when you select photos, create and save cards, export your work, and use purchase features. LiveCard processes photos and creates cards on your device. No LiveCard account is required. The current app has no feature that uploads your photos or cards to a developer-operated server.

## 2. Photos and subject processing

You select photos through Apple's system photo picker. LiveCard receives the content you select and does not independently scan your entire photo library. If a selected photo is stored in iCloud, the system may need to download it through Apple's services.

LiveCard performs framing, cropping, subject segmentation, and visual rendering on your device. It uses Apple Vision to create subject masks, outlines, and position data. This data places effects around the subject; it is not used to identify people, build facial identity profiles, or train the developer's AI models. Photos and subject data are not sent to a developer-operated server for these operations.

When you save a card, the app stores its image, subject mask and outline, card name, creation time, effect and border settings, and ordering information locally. The current card creation flow renders a new cropped image without deliberately copying the original photo's EXIF metadata. Existing cards may retain image data and embedded metadata saved by earlier versions.

## 3. Local settings, storage, and backups

Cards are stored in the app's data directory on your device. Trial-use counts and display preferences are also stored locally to maintain your collection and app state, not for advertising or cross-app tracking.

The app does not provide its own cloud collection sync. Device backups may include local app data, depending on Apple's backup mechanisms and your settings. Works saved to the system photo library may also sync through iCloud Photos. You can manage these services in system settings. On-device processing therefore does not mean your data can never enter system backups or cloud services you enable.

## 4. Export, photo permissions, and sharing

When you export, LiveCard creates temporary image and video files on your device and makes them available through the system share sheet. Opening the share sheet does not automatically save your work to your photo library. Choosing “Save Live Photo” requests permission to add content to your photo library. Denying this permission prevents saving to the library but does not affect local storage of existing cards.

When you choose a recipient or another app, the selected content is provided to that recipient or service. Their policies and your settings govern further handling. Shared content may include personal information visible in the photo. Check the content and recipient before sharing.

## 5. In-app purchases and restoration

In versions with App Store purchases enabled, purchases and restoration use Apple StoreKit. Apple handles payment and Apple Account authentication. LiveCard does not receive your full payment-card number or Apple Account password. The app reads product and verified transaction information supplied by Apple, including product identifiers, transaction identifiers, purchase entitlements, and revocation or validity status. This information unlocks features, restores purchases, and updates access; it is not uploaded to a developer-operated server.

When you choose to restore purchases, the app requests synchronization with the App Store, and Apple may ask you to authenticate. The app may also check entitlements at launch, when returning to the foreground, and when transaction updates arrive. Restoring purchases does not restore locally saved cards or photos.

The current development version does not have live products configured. Confirm this section against the purchase features actually released before publication. Local StoreKit testing does not involve real payment.

## 6. Diagnostics, advertising, and tracking

The current version includes no third-party advertising, behavioral analytics, or crash-reporting SDK, and no cross-app advertising tracking feature. When subject recognition fails, the app writes an error description to the system log. The app does not itself upload these logs to a developer-operated server.

Apple may process system diagnostics, crash information, and App Store service information according to system settings and its policies. This is separate from the app's photo processing. This policy does not replace the privacy information provided by Apple or sharing services you choose to use.

## 7. Retention, deletion, and your choices

Saved cards remain locally until you delete them or remove the app's data. Deleting a card in the card editor removes its local archive. The ordering file may temporarily retain a deleted card's random identifier, but not its image. The app attempts to remove temporary export files when no longer in use. Files left after an unexpected exit may be cleaned up later by the system.

Deleting a card in LiveCard does not delete original photos, exported works in your photo library, recipients' copies, system backups, or Apple's transaction records. Manage those items separately in the relevant app or service. System “Offload App” options may retain data, while “Delete App” normally removes local app data. Backup copies must still be managed separately. The app relies on operating-system access protections; absolute security cannot be guaranteed.

You can choose not to select photos, save, or share, and manage available photo permissions and backup settings through the system. For privacy questions, use the contact address above. Please do not send unnecessary photos or sensitive information when contacting us.

## 8. Policy webpage

This policy is intended to be published through GitHub Pages. When you visit a GitHub Pages site, GitHub logs and stores your IP address for security purposes, whether or not you are signed into GitHub. See the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). This draft is not yet effective as the final policy. Before publication, we will check that the page does not introduce additional analytics scripts, third-party fonts, or advertising.

## 9. Policy changes

This policy needs to be updated if information handling changes. The published version will include an effective date and an accessible location for the current policy.

[Before publication, confirm: distribution regions, intended age group, and any required children's privacy or local privacy-rights and request procedures; the final policy URL and whether the webpage adds any other information-processing features.]
