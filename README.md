vtiger-customer-portal-german
=============================

German translation for vtiger customer portal.

##Installation
First copy de_de.lang.php into the vtiger customer portal language directory.

    cd CUSTOMERPORTAL_ROOT
    git clone https://github.com/chanzler/vtiger-customer-portal-german.git
    cd vtiger-customer-portal-german
    mv de_de.lang.php ../language
    cd ..
    rm -r vtiger-customer-portal-german

Next step is to configure the customer portal to use the new language file. go to your CUSTOMERPORTAL_ROOT directory and edit PortalConfig.php

Now replace
 
    $languages = Array('en_us'=>'US English');

with

    $languages = Array('en_us'=>'US English','de_de'=>'Deutsch');

If you want to set the german language as your default language them replace

    $default_language = 'en_us';

with 

    $default_language = 'de_de';

Voila, that's it. Go to your customer portal and you will be able to chose the german language.