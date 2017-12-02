Migration script vih.dk
--

    drush si
    drush sqlc < ../dump-til-lars.sql
    drush en custom_migrate --yes
    drush mim --all --yes --update
    drush mr --all --yes
    