# eclinux.org
Website for the Emerald Coast Linux User Group.

## Hugo Development
This site is made in Hugo. To work with this site locally:
1. Clone the Repository
2. Change into the *docker-compose* directory.
3. Run the following command to start a Hugo server locally for testing:
   
   ```docker compose -f server.yml up```

You can then access the site in via http://localhost:1313/ in a web browser.

## Committing Changes
This site will be hosted with [netlify](https://www.netlify.com/). Changes that are approved via this Github repo are automatically put into production.