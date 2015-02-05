# CF-CertMan

An extension for ColdFusion Administrator that allows adding/viewing/removing of SSL certificates in the Java certificate store from within the Administrator.

This works with ColdFusion versions 7, 8 & 9. For a CF10 version please check out [CF10-Certman](https://github.com/coldfumonkeh/CF10-Certman).


## Installation

Extract the contents of this repository into a CFIDE/administrator/certman/ directory.

In ColdFusion 8/9 - Edit the CFIDE\administrator\custommenu.xml file to add the following submenu xml key:-

    <submenu label="SSL Certificates">
      <menuitem href="certman" target="content">Certificate Management</menuitem>
    </submenu>

  You can only use this extension in a multiuser admin environment when logged in as the administrator user.


In ColdFusion 7 - Create/Edit CFIDE\administrator\extensionscustom.cfm to add:-

    <a href="certman" target="content">Certificate Management</a><br>


### Notes

The CertMan project was originally developed by Paul Connell.

This is a fresh fork taken to separate the specific ColdFusion versions for easier use.
