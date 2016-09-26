INSTALLATION
------------

Gulp is required to compile and manage assets properly.

1. Install NodeJS on your development machine and ensure you can run the 'npm' command.
2. Install the Gulp CLI globally with 'npm install --global gulp-cli'
3. Create a subtheme from Spacelift. See the BUILD A THEME WITH DRUSH section below for more information.
4. In your subtheme directory, copy 'default.config.json' to 'config.json' and configure the theme compilation settings.
5. From within your subtheme directory, run 'npm install' on the command line.
6. From within your subtheme directory, run 'gulp' to start the default watch task, or 'gulp --tasks' to see a list of all possible tasks.

When the 'watch' task is running, saving any watched files (such as src/scss/*.scss or src/scss/*.js) will trigger a re-compile and clear the cache if you have Drush integration enabled.

You may customize Gulpfile.js as you see fit to modify or add your own compilation steps.

BUILD A THEME WITH DRUSH
----------------------------------
It is highly encouraged to use Drush to generate a sub theme for editing. Do not edit the parent 'spacelift' theme!

  1. Enable the Spacelift theme and set as default. You can unset it as default after you are done step 2.
  2. Enter the drush command: drush sgt [THEMENAME] [Description !Optional]
