Web App Cookbook
=======================
Installs tools for LAMP based web application development.   

Cookbooks
---------
- apache
- iptables  

Attributes
----------

- `node[['webapp']['vhost']` = apache vhosts files to create e.g. 

node['webapp']['vhost'] = {  
  :site1 => {
      :name => "site1",
      :host => "site1.local", 
      :aliases => [site1.test.local],
      :docroot => "/site1"
    },
    :site2 => {
      :name => "site2",
      :host => "site2.local", 
      :aliases => [site2.test.local],
      :docroot => "/site2"
    }
}
