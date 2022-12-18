# How to Post Your Mastodon Link on Twitter

## Step 1) Create a Subdomain and Webspace

Create a subdomain on your hosting with your own domain. I created **mastodon.hereticerik.com** and pointed it to a webspace called /mastodon

## Step 2) Edit this index.html File.

Edit this **index.html** file and change the meta refresh tag to point to your Mastodon URL, and change the text to say "loading <your username>'s profile..."

## Step 3) Upload this index.html file to your webspace.

Upload this edited index.html file to your webspace, and you're good to go! You can now post your subdomain link to your twitter and share your mastodon link!

## Additional Tips

If you want to force HTTPS on your subdomain/mastodon link (strongly suggested) then add the .htaccess file included to your webspace directory. 

Contents of .htaccess

```
RewriteEngine On
RewriteCond %{HTTPS} !=on
RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301,NE]
Header always set Content-Security-Policy "upgrade-insecure-requests;"
```

###### Enjoy posting your mastodon link to your twitter account. ;) 
