Wildframe photo folder
======================

All photographs live in this folder. The portfolio page reads them from here.

HOW TO ADD, REPLACE OR REMOVE A PHOTO
-------------------------------------

Add a new photo
  1. Copy the image into this images/ folder (JPG recommended, about 1500 px on the long side).
  2. Open "Wildframe Wildlife Studio.html" in a text editor.
  3. Find the list that starts with  var PHOTOS = [  (inside the <script> at the bottom).
  4. Add one line, copying an existing one:

     { file: 'new-photo.jpg', alt: 'Short description', title: 'Photo title', place: 'Location · Note', category: 'birds' },

  5. Save and refresh the page. The photo appears in the gallery automatically.

Replace a photo
  - Save the new image in this folder with EXACTLY the same file name (overwrite the old one).
  - No change to the HTML is needed. Refresh the page.

Remove a photo
  - Delete its line from the PHOTOS list in the HTML.

Add a new category (for example "Reptiles")
  - Add it to the CATEGORIES list in the HTML, e.g. { id: 'reptiles', label: 'Reptiles' },
  - Use id 'reptiles' as the category on the photos that belong to it.

PORTRAIT AND LANDSCAPE
----------------------
- No size setting is needed. The page checks each photo and frames it automatically:
    landscape photos  -> 3:2 frame
    portrait photos   -> 4:5 frame
- The gallery is a masonry layout, so portrait and landscape photos sit together without gaps.
- Keep the main subject near the centre. The frame crops the edges to fit.

HERO PHOTO (home page)
----------------------
  hero-bengal-tiger.jpg      Replace this file (same name) to change the hero image.
                             The hero frame is 4:5 portrait.

NOTES
-----
- Until a file exists, the coloured placeholder shows in its place, so nothing breaks.
- The list works when you open the HTML file directly. No server or internet connection is needed.
- Keep file names in lowercase, with hyphens instead of spaces (for example: sloth-bear.jpg).
