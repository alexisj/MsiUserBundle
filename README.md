Installation :

Add MsiUserBundle :

    git submodule add -f git://github.com/alexisj/MsiUserBundle.git vendor/bundles/Msi/UserBundle

Add to kernel :

    new Msi\UserBundle\MsiUserBundle(),

Register namespace :

    'Msi'  => __DIR__.'/../vendor/bundles',

Add to routing :

    MsiUserBundle:
      resource: "@MsiUserBundle/Resources/config/routing.yml"

Install assets

    app/console assets:install --symlink web