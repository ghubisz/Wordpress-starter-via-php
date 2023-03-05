WordPress Project Template is a skeleton WordPress site with modern development tools, easier configuration, improved folder structure and latest security best practices.

The organization of skeleton is similar to putting WordPress core files in its own subdirectory, wp-content stays the same.

Manage your WordPress install and plugins with Composer, a PHP dependency manager. Composer will make development more reliable, help with team collaboration, and it helps maintain a better Git repository.

Easy WordPress configuration

Environment specific configuration files and environment variables with Dotenv.
Important plugins out of the box

The package has some pre-defined plugins already installed (they will be downloaded through installation automatically). We included most popular plugins for SEO, better editing experience, SMTP support, etc.

Enhanced security

    Deny access to non-web files with server directives (with .htaccess files).
    Deny PHP scripts execution inside wp-content/uploads folder.
    Deny browsing the directory files list.
    Production & Staging environments have a restriction to update files from admin panel (only Media is allowed).
    Command-line scripts for generating wp-admin HTTP Authorization files.

* Note: Works for LAMP stacks with mod_rewrite enabled (most popular server configuration).

Quick start
Requirements

    PHP >= 7.0
    Composer
    Installation

    Create a new project in a new folder for your site:

composer create-project justcoded/wordpress-starter your-project-folder-name

    Set important environment variables in .env file:

    DB_NAME - Database name
    DB_USER - Database user
    DB_PASSWORD - Database password
    DB_HOST - Database host
    WP_HOME - Full URL to WordPress home (http://example.com)

    Run WordPress install as usual by accessing your site at http://example.com/

    Enjoy!

Composer helpers

    composer wp:theme generate new theme based on our Theme Boilerplate
    composer wp:secure generate new HTTP password for wp-admin folder


