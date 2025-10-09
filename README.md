# PHP Plugin to Integrate Postal with Mautic

Integrate Postal Email service with Mautic to send emails via API.

> Notes:
>
> Mautic 5.x is not supported at this time

## Installation

### Manual Mode

-   Go to the plugins folder on Mautic add a new folder called
    `MauticPostalServerBundle`

```shell
mkdir /mautic_path/plugins/MauticPostalServerBundle
```

-   Go inside the folder and clone the repo

```shell
cd MauticPostalServerBundle
git clone https://github.com/LucasCCS/postal_server_api_transport_for_mautic.git .
```

-   Reload the plugin list

```shell
rm -rf /mautic_path/var/cache/*

php /mautic_path/bin/console mautic:plugins:reload
```

-   Got to your Mautic plugins menu (`https://mauticURL.com/s/plugins`), and you
    should see the plugin there. If you dont see it, click the
    `Install/Upgrade Plugins` button.

### Via composer

-   Go to the your mautic folder and run

```shell
cd /mautic_path
composer require lucascosta/postal-server-api-transport-for-mautic
```

## How to use it

-   Once the plugin is installed, go to the email settings on your Mautic server
    (`https://mauticURL/s/config/edit`), you should see `Postal -API` as a new
    item you can select from the drop-down menu.

-   Provide the Postal email server name and the API key you generated and click
    on save.
