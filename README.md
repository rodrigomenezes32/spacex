# spacex
Wordpress Spacex Launches and history website.

This project consists on pulling Data from a Spacex API and displaying it for the user on the Pages Launches and History.

This programm runs on funtion.php inside the theme Screenr.

I used the plugin ACF Custom fields to create custom fields inside posts to match with the API Data.

Using wp_remote_retrieve_body( wp_remote_get('https://api.spacexdata.com/v3/launches') );

to grab the data, and using json_decode to transform the data and insert into posts using wp_insert_post. 

Also ran a variable with arrays to pass each wanted field inside the custom fields on a foreach loop.

Next step will be reading those posts and printing on those pages on an organized way.

