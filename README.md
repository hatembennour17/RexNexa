VS Code Live Server

Install Live Server

Right-click index.html → Open with Live Server


How you “edit” it as admin (no backend)

Go to /admin.html

Enter password (ChangeMe123!)

Click Load current JSON

Edit text + image paths (ex: uploads/screen4.png)

Click Download site.json

Upload and replace your hosted content/site.json

Upload images into /uploads/

That’s it.


This is no-backend, so the admin page cannot directly write to server files on Tiiny/static hosting. Static hosting doesn’t allow that.

The admin page is a content editor + exporter (the most reliable “no backend” approach).

If you later want “save live changes” without building a backend, the clean upgrade is: save JSON to GitHub via API or use Cloudflare KV / Supabase storage (still “no backend you manage”, but adds a service).
