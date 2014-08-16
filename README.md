# Nginx Wildcard Domain

This is designed to serve static sites without having to update a config file every time you want to
host a new site. The sites should be put in `/var/www/sites/a.domain.com`, and files will be served
from `/var/www/sites/a.domain.com/dist`.

(This pairs up with a gitolite based continuous deployment system, forthcoming...)

The work is done in [sites-available/wild_domain](sites-available/wild_domain).

Based on the default Ubuntu nginx configuration.

[nginx.conf](nginx.conf) is also tweaked for performance and to remove cruft.

## Contributing

You can tell me whether `scgi_params` and the like are necessary. I am too cowardly to remove them.
