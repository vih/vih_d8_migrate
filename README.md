Migration script vih.dk
--

Copy images from the old site to ´sites/default/files/import´.

Reinstall the site using these commands.

    drush si --yes && drush sqlc < ../dump-til-lars.sql && drush en custom_migrate --yes && drush mim --all --yes && drush mim --all --yes --update

Utilize these commands to import content, if you need to update them.

    drush mim --all --yes --update
    drush mr --all --yes
