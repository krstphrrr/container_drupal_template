FROM drupal:latest

# getting vim inside the container for development/troubleshooting
RUN apt-get update \
    && apt-get install vim -y

# local drush ( local with respect to the drupal install; not global)
RUN composer require drush/drush 
# making sure the drush path is available
RUN export PATH="$HOME/.composer/vendor/bin:$PATH"

