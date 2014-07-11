panamax-docker-drupal
=====================

Out-of-the-box Drupal docker image without a DB included in the image. This image is designed to be used with panamax/panamax-docker-mysql or similar stand-alone DB image in order to create a multi-container cluster. 

On docker run, browse to Port 80 to do initial setup. 
Example usage:

<pre><code>docker run --rm --name DRUPAL --link DB:DB panamax/panamax-docker-drupal:7.28
</code></pre>

...where `DB:DB` matches the name and alias of your DB instance. Use the values from your linked DB image to complete GUI setup.
