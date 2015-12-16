# to serve the static content locally, in the output directory
$ python -m SimpleHTTPServer

# to re-generate static files from the content directory
$ pelican content

# to publish, after git commit
$ ghp-import output
$ git push git@github.com:devcurmudgeon/devcurmudgeon.github.io.git gh-pages:master -f~/Projects/2015/devcurmudgeon>ls
