Project setup instructions

To setup current WordPress project, you should do the following steps: (Project is based on WordPress Starter )
Navigate to project and clone git repo:

cd /path/to/your/project/empty/folder/
git clone http://repository-domain.com/your/project.git

Switch to latest branch

    master - stable production copy,
    develop - current development copy

git checkout <branch-name>

Download wp core with composer

composer update

(if you don't have composer installed on your machine you can download php script: https://getcomposer.org/download/)
Create new branch for your changes

git checkout -b {issue#}_{short descr}

Create your environment

    Update environment variables in .env file:

    DB_NAME - Database name
    DB_USER - Database user
    DB_PASSWORD - Database password
    DB_HOST - Database host
    WP_ENV - Set to environment (development, staging, production)
    WP_HOME - Full URL to WordPress home (http://example.com)

Database setup (Dev environment ONLY)

    Download latest database dump from repository "Downloads" section (Bitbucket)
    Import sql dump to your database
    Upgrade URLs inside database with any method you like the most: WP Host update, WP Migrate, WP CLI

