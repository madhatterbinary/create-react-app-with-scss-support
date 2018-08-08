# Customize create-react-app without ejecting using react-app-rewired

npm install --save react-app-rewired

npm install --save sass-loader node-sass 

create a config-overrrides.js file at the root level

go to node_modules/react-scripts/config/webpack.config.dev and webpack.config.prod

search for comment:

// ** STOP ** Are you adding a new loader?
// Make sure to add the new loader(s) before the "file" loader.

In your config-overrrides.js clone a new loader with your additional configuration at the location #  and return the new config object: let loaders = config.module.rules[1].oneOf;



     
     
