# webapp

<ol>
  <li>Clone the repo</li>
  <li>Install the packages using <kbd>npm install<kbd></li>
  <li>Run using <kbd>ionic serve -lab</kbd></li>
</ol>

Here is how to use angular-cli-ghpages with Ionic 4:

    Create your Ionic project (ionic start MyApp blank)
    Install the plugin: npm i angular-cli-ghpages --save
    Connect your project with your github repository.
    Navigate in the terminal to your project directory and execute ionic build --prod -- --base-href https://YOUR_GITHUB_USERNAME.github.io/YOUR_PROJECT_NAME/, what will create the www folder, which is comparable to the dist folder for Angular. It also sets your github page domain as base href in index.html.
    Then run the plugin: npx angular-cli-ghpages --dir=www. The flag at the end points to the www folder, where the index.html file is located that will be displayed at https://YOUR_GITHUB_USERNAME.github.io/YOUR_PROJECT_NAME/. The plugin will create a branch called "gh-pages" in your project that contains all files which are located in your www folder.
    As a last step you have to select the "gh-page" branch in the settings of your project (https://YOUR_GITHUB_USERNAME.github.io/YOUR_PROJECT_NAME/settings) as a source for your github page.

You can also set different branch names if you don't want to use the default "gh-pages" name (also master is possible, but then you should keep the source files in a different branch). Just run the plugin like this: npx angular-cli-ghpages --branch=BRANCH-NAME --dir=www.
