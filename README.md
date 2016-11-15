## vflex.js

A simple script to style Visualforce page tags with the Salesforce Lightning Design System 

1. Download the Lightning Design System [zip file](https://www.lightningdesignsystem.com/assets/downloads/salesforce-lightning-design-system-2.1.4.zip)

1. Create a static resource named `slds` and select the Lightning Desing System zip file
 
1. Create a static resource called `vflex` and upload the `vflex.js` file in this repository
 
1. In the Developer Console, create a new Visualforce page named `VFSample1`. Paste the code from the VFSample1.vfp file in this repository. Examine the page and notice:

    - `standardStylesheets="false"` on the `apex:page` tag, indicating that the Salesforce Aloha styles shouldnot be applied
    - `<script src="{!URLFOR($Resource.vflex)}"></script>` as the last line before the closing body tag to load the vflex script.
  
1. Preview the page