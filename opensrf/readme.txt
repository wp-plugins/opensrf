=== Opensrf_PHP ===
Contributors: pranjalprabhash
Tags: PHP
Requires at least: 3.3
Tested up to: 3.5.1
License: LGPL
License URI: http://www.gnu.org/copyleft/lgpl.html

The Open Service Request Framework (or OpenSRF, pronounced “open surf”) is an inter-application message passing architecture built on XMPP (aka “jabber”). The Evergreen open source library system is built on an OpenSRF architecture to support loosely coupled individual components communicating over an OpenSRF messaging bus

== Description ==
(extracted from **http://journal.code4lib.org/articles/3284*)*

OpenSRF is a message routing network that offers scalability and failover support for individual services and entire servers with minimal development and deployment overhead. You can use OpenSRF to build loosely-coupled applications that can be deployed on a single server or on clusters of geographically distributed servers using the same code and minimal configuration changes. Although copyright statements on some of the OpenSRF code date back to Mike Rylander’s original explorations in 2000, Evergreen was the first major application to be developed with, and to take full advantage of, the OpenSRF architecture starting in 2004. The first official release of OpenSRF was 0.1 in February 2005 (http://evergreen-ils.org/blog/?p=21), but OpenSRF’s development continues a steady pace of enhancement and refinement, with the release of 1.0.0 in October 2008 and the most recent release of 1.2.2 in February 2010.

OpenSRF is a distinct break from the architectural approach used by previous library systems and has more in common with modern Web applications. The traditional “scale-up” approach to serve more transactions is to purchase a server with more CPUs and more RAM, possibly splitting the load between a Web server, a database server, and a business logic server. Evergreen, however, is built on the Open Service Request Framework (OpenSRF) architecture, which firmly embraces the “scale-out” approach of spreading transaction load over cheap commodity servers. The initial GPLS PINES hardware cluster, while certainly impressive, may have offered the misleading impression that Evergreen requires a lot of hardware to run. However, Evergreen and OpenSRF easily scale down to a single server; many Evergreen libraries run their entire library system on a single server, and most OpenSRF and Evergreen development occurs on a virtual machine running on a single laptop or desktop image.


== Installation ==

1. Upload `plugin-name.php` to the `/wp-content/plugins/` directory
2. HTTP_Request2 should be present
3. Activate the plugin through the 'Plugins' menu in WordPress
4. Works for OpenSRF service running on localhost, for service running on other host, please change "hostname" in config.php.