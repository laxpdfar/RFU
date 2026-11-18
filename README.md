# RFU
LAXPD Rescue follow up

## Injury Report – Fill-in App

A one-page web app for filling out the Airport Police Division **Injury Report (APB Form 045)** on a phone, tablet or computer.

### Features

- Every field from the paper form, in 11 sections
- **Scan ID**: reads the barcode on the back of a US/Canadian driver's license or state ID and fills in the victim's details
- **Photos**: take or attach photos, with captions; they're added to the end of the report
- **Dictate the narrative** (Chrome, Edge and Safari)
- Dropdowns for reporting officer (with serial number), supervisor and airline
- **Download report** as a Word file: the original APB Form 045 with every field filled in (photos are added on pages at the end)
- **Submit to supervisor**: downloads the Word file and opens a pre-filled Outlook email; on phones you can share the Word file straight to Outlook with it already attached
- Drafts save automatically in the browser; **Save form data** / **Open saved…** move a report between devices

### Using it

Open the site and fill in the form. Nothing is sent anywhere by the app itself: the form data, photos and drafts stay in the browser on that device until you download or email the report.

### Updating the lists

The officer, supervisor and airline lists are `<option>` entries inside `index.html` (search for `id="ofc"`, `id="sup"` and `id="arr_airline"` / `id="dep_airline"`).

### Hosting

The whole app is the single file `index.html`. With GitHub Pages turned on (Settings → Pages → Deploy from branch → `main` / root), it is served at https://laxpdfar.github.io/RFU/.
