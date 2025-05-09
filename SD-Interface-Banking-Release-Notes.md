## SD Interface Banking Releases

### 5.1.0

#### Enhancements

- AppSource App - The length of the Company Information Name in the EndToEndID for AIB Credit Transfer formats can not exceed 35 characters. The SEPA CT pain.001.001.03 AIB and SEPA CT pain.001.001.09 AIB formats were updated to reflect this.

- AppSource App - A new Licence Install and Setup Wizard was created.

- AppSource App - Changes were made to the Manage Subscriptions page.

- AppSource App - The notification to activate the app, displayed on fresh install of SD Interface Banking, was added to the standard Business Central role centres.

- AppSource App - A minor change was made to the About page.

### 5.0.0

#### Enhancements

- AppSource App - The OIN Number for some of the SEPA Credit Transfers formats was picked up from the Payment Routing number on the Company Information Card, the Vat Registration No on the Company Information Card or the Bank Clearing Code on the Bank Account Card. A change was made to handle situations where Credit Transfers will be sent from more than one bank. The OIN is now picked up from the Transit No. on the Bank Account Card for the following XMLports 43015111 SDY INBK pain.001.001.03 AIB, 43015115 SEPA CT pain.001.001.09 AIB, xmlport 43015113 SDY INBK SEPA CT AIB USD, xmlport 43015121 SDY INBK SEPA CT BOI, xmlport 43015107 SDY INBK ACH DD CITI, xmlport 43015161 SDY INBK Citibank SEPA CT, xmlport 43015160 SDY INBK Citibank WIRECT, xmlport 43015131 SDY INBK SEPA CT Danske, and xmlport 43015101 SDY INBK pain.001.001.03 ULS.

- AppSource App - For the SDBK-DABA-BACSCT format the mandatory requirement on IBAN was removed. Also, the Transit No is now picked up from the Bank Account Card and not the Vendor Bank Account.

- AppSource App - A change was made to XMLport 43015111 SD-INBK CT pain.001.001.03 AIB to populate the EndToEndId with the Company Information Name.

- AppSource App - A new SDBK-BOFI-CT-V09 format for BOI SEPA CT Pain 001.001.009 was created.

- AppSource App - New XMlports were created for SEPA CT pain.001.001.09 AIB and SEPA DD pain.008.001.08 AIB. The EndToEndId in the SEPA CT pain.001.001.09 AIB is also populated with the Company Information Name.

- AppSource App - The bank connectivity was reworked to allow for direct file transfer between Business Central and a bank's SFTP server.

- AppSource App - The need to transfer bank files to/from blob storage and then to/from SFTP was removed. Bank files are now transferred directly using SFTP. 

- AppSource App - H2H Tables and Functionality was made obsolete.

- AppSource App - New tables and functionality added for banking connectivity - SDY INBK File API Request, SDY INBK File To Bank, SDY INBK File To Bank Archive and SDY INBK File From Bank.

- AppSource App - All bank file transfers via SFTP are now per company.

- AppSource App - The underlying structure of the bank file status KPIs were reworked. New tables and pages were created.

- AppSource App - Three new cues were added to the Role Centre Files Pending, Files Processed and Files Rejected.

- AppSource App - A new Bank File Status FactBox was created that shows the time the file was created, sent to the bank, acknowledged and either accepted or rejected.

- AppSource App - UI Changes were made to the SFTP Connection Card.

- AppSource App - Functionality was added to allow for manual upload of a bank statement to the Pending Bank Files list.

- AppSource App - Functionality was added to log the manual creation of Credit Transfer and Direct Debit files to the File To Bank Archive table for files that will not be sent to the bank via SFTP.

- AppSource App - Changes were made to the extension of the Bank Export/Import Setup List to allow for users to easily see which bank formats are active on their banks. 

- AppSource App - A new action was added to the Setup Card called View Our Apps. This action opens a page on AppSource pointing to all our Simply Dynamics Ltd apps.

- AppSource App - The Lead Subscription Link from the Request Subscription action in the Product Activation page was updated.

- AppSource App - The data inserted when the Apply Default Setup is chosen was updated.

- AppSource App - Minor changes were made to the extended Customer List (22, List) and Vendor List (27, List) surfaced on the SD Interface Banking Activities. The default filters were updated.

- AppSource App - An extension to the Direct Debit Collections (1207, List) was created and is surfaced on the SD Interface Banking Activities. 

### 4.0.3

#### Enhancements

- AppSource App - A change was made to the licence expiry notification. The logic for checking for expiry dates was reworked.

- AppSource App - Enhancements were made to the App Request Subscription page.

- AppSource App - Additional phrases were added as search phrases for the SD Interface Banking pages.

- AppSource App - ToolTips were updated in the About, Product Activation, and Tenant Subscription pages.

- AppSource App - The Banking Activities Card was updated to reflect the cues in the SD Interface Banking Role Centre.

### 4.0.2

#### Enhancements

- AppSource App - Changes were made to the MT940 Statement Import format to handle "DN" line types.

#### Bug Fixes

- AppSource App - An SD Interface Banking Mapping Bank Account No. field was referenced in the MT940 Statement Import format. This field was not used in any of the other bank formats and is now marked as obsolete as it was causing an error on import of statements using the MT940 Statement Import format.

### 4.0.1

#### Enhancements

- AppSource App - A change was made to allow import of xml files using the standard SEPA statement import.

- BCv14 App - A change was made to Codeunit 43015111 SD-INBK CT pain.001.001.03 AIB to populate EndToEndId with Company Information Name.

### 4.0.0

#### Enhancements

- AppSource App - A second AIB Statement Import Definition Exchange File was created and a new record added to the Bank Export/Import Setup. The definition of the AIB statement import can vary.

- AppSource App - A format for AIB SEPA CT Payment for USD was created and a new record in the Bank Export/Import Setup was created. 

- AppSource App - A SEPA CT format for HSBC was added and a new record added to the Bank Export/Import Setup.

- AppSource App - A SEPA Urgent (Faster) CT format for HSBC was added and a new record added to the Bank Export/Import Setup.

- AppSource App - A new Data Exchange Definition was created for Barclay's statement import and a new record added to the Bank Export/Import Setup.

- AppSource App - A second Danske Bank Statement Import Definition Exchange File was created and a new record added to the Bank Export/Import Setup. The definition of the Danske Bank statement import can vary.

- AppSource App - An SD Interface Banking Setup card was created. 

- AppSource App - The SD Interface Banking format codes, populated when the Apply Default Setup action in the Setup card is selected, were normalised to use the individual bank's standard bank code.

- AppSource App - A FactBox was added to the Bank Export/Import page to surface a column count to show the banks the format is applied on and allow drill through to the list of banks. The Faster Payments, and Decimal Indicator option fields were also added to this FactBox as was a link to the Blob Storage Setup.

- AppSource App - The SD Banking Interface Assigned field was hidden on the Bank Export/Import Setup as the field is used to determine which records are standard and which have been populated by SD Interface Banking. 

- AppSource App - Actions were surfaced in the SD Interface Banking Setup card to allow users to navigate to the H2H Blob Storage Setup and to the SFTP Connections Setup.

- AppSource App - The links in the About Page were updated.

- AppSource App - The logo in App was updated to the new logo.

- BCv14 App - Integration to GoCardless was added to the BCv14 App.

### 3.0.2.7

#### Bug Fixes

- BCv14 App - A fix was made to the Citibank BACS Direct Debit format. 

### 3.0.2.6

#### Enhancements

- BCv14 App - A change was made to the namespace for the Citibank BACS Direct Debit format.

### 3.0.2.1

#### Enhancements

- BCv14 App - A minor modification was made to the Citibank BACS DD format.

### 3.0.2

#### Enhancements

- BCv14 App - The format for Citibank BACS DD was updated to output Bank Sort Code and Bank Account Number.

### 3.0.1

#### Enhancements

- BCv14 App - A number of small fixes for H2H Connectivity were made.

### 3.0.0

#### Enhancements

- AppSource App - H2H Connectivity was added to SD Interface Banking. Blob Storage Setup tables, pages and codeunits were created. SFTP Interface tables, pages and codeunits were created. An Azure Function Template was created to manage traffic between Blob Storage and SFTP. Cues were added to the SD Interface Banking Role Centre for inbound file list, outbound file list, blob storage setup, and SFTP connections.

- AppSource App - Citibank ACH DD was added to SD Interface Banking.

- BCv14 App - Blob Storage Setup Tables, Pages and Codeunits were created for H2H connectivity in SD Interface Banking.

- BCv14 App - SFTP Interface tables, pages and codeunits were created for H2H connectivity in SD Interface Banking.

- BCV14 App - An Azure Function Template was created to manage traffic between Blob Storage and SFTP.

- BCv14 App - Cues were added to the SD Interface Banking Role Centre for inbound file list, outbound file list, blob storage setup, and SFTP connections.

### 2.2.1

#### Enhancements

- AppSource App - A change was made to limit the SD ISV Tenant Subscriptions page to display just our SD ISV AppSource Apps and not other SD PTE Apps.

#### Bug Fixes

- AppSource App - When selecting SD Interface Banking activity pages in a the Tell Me/Search in a BCv22 environment, the activity pages were hanging.

### 2.2.0

#### Enhancements

- BCv21 App - A change was made to the standard SEPA CAMT for Barclays SEPA CAMT. An event was added that removes a tag in the file. This change does not affect other banks using the SEPA CAMT format as those files will not have this tag. 

- BCv21 App - Citibank SEPA DD was added to SD Interface Banking.

- BCv21 App - Citibank SEPA Statement was added to SD Interface Banking.

- BCv21 App - NatWest Statement was added to SD Interface Banking.

- BCv21 App - NatWest SEPA Credit Transfer format was added to SD Interface Banking.

- BCv21 App - BNP SEPA Credit Transfer and SEPA CT GBP formats were added to SD Interface Banking.

- BCv21 App - HSBC Credit Transfer BACS 18 Format was added to SD Interface Banking.

- BCv21 App - MT940 and MT940N Statement file formats have been added to SD Interface Banking.

#### Bug Fixes

- BCv21 App - A change was made for NatWest SEPA CT. A Payment Type of 01 or 04 has been added to the Vendor Bank Account Card and when the payment journal is created the Payment Type field is added to the journal. Bank details are formatted in the outputted file depending on the value of the Payment Type field.

- BCv21 App - A change was made to the PTX CT files to create Credit Transfer Register and Credit Transfer Entry records.

- BCv21 App - Some extra nodes were added to the BOI SEPA Credit Transfer format.

### 2.1.0

#### Enhancements

- BCv21 App - The ISV Licence Controller was added to SD Interface Banking. 

- BCv21 App - A change was made to add a licence message on first install of SD Interface Banking to prompt the user to activate a free trial and to choose the Apply Default Setup action from the Role Centre to populate Bank Export/Import Setup. 

- BCv21 App - A page was created to display all the Simply Dynamics Apps and subscription details for the tenant. 

- BCv21 App - The Licence Expiry message/notification was updated to display the App Name as part of the message. 

- BCv21 App - Permission set xml files were replaced with an AL Permission object. 

- BCv21 App - ToolTips were updated to point to our new website and not the old. 

- BCv21 App - The URL links in the About page were updated to point to our new website and not the old. 

- BCv21 App - The About page was updated to display the Latest Version of the App and the URL link to SD Interface Banking on AppSource. 

- BCv21 App - The default data codeunit was removed from running at App Install and is now surfaced as an action Apply Default Setup on the SD Interface Banking Role Centre. 

- BCv21 App - BOI BACS CT files were added to SD Interface Banking.  

- BCv21 App - The BOI setup was added to the SD Interface Banking Apply Default Setup function. 

- BCv21 App - RBS Statement Import XMLports were added to the product. 

- BCv21 App - The RBS Statement Import setup was added to the SD Interface Banking Apply Default Setup function. 

- BCv21 App - Citibank files for Citibank BACS CT, SEPA CT, WIRE CT were added to the App. 

- BCv21 App - The Citibank setup was added to the SD Interface Banking Apply Default Setup function. 

- BCv21 App - A change was made to the Barclays SCT MT103 to export the Vendor name and Address instead of the Bank Address. 

- BCv21 App - For the Barclays BACs Credit Transfer a change was made to stamp the Destination Account Name to the Vendor Name.  

- BCv21 App - Changes were made to the PTX setup to allow for export of files using a Codeunit or an XMLport. This allows for flexibility for sites to create their own xmlports for export to csv to allow for easy implementation of site variations. 

- BCv21 App - An option was added to the Bank Export/import Setup to flag a Danske BACS CT as a Faster Payment. 

#### Bug Fixes

- BCv21 App - A fix was made to the Direct Debit collection split amount functionality.  When the "Split Amount" action is selected on the DD Collection Entry and the DD Entry Status is validated as "File Exported", then the CLE Due Date is updated to the date as specified in the DD Split Amount Setup. 

- BCv21 App - Barclays MT103 - The "Bank code" check was removed from the export check codeunit, 

- BCv21 App - A fix was made to the Data Exchange Definition for the BOI Statement import. 

### 2.0.7

#### Bug Fixes

- BCv14 App - A fix was made to the Direct Debit collection split amount functionality.  When the "Split Amount" action is selected on the DD Collection Entry and the DD Entry Status is validated as "File Exported", then the CLE Due Date is updated to the date as specified in the DD Split Amount Setup.

### 2.0.6

#### Enhancements

- BCv14 App - The Transfer Date on the Direct Debit Collections page was amended.

- BCv14 App - Change to PT-X (Bottom Line Technology) BACS CT - values must contain no decimal points.

- BCv15 App - Change to PT-X (Bottom Line Technology) BACS CT - values must contain no decimal points.

- BCv16 App - Change to PT-X (Bottom Line Technology) BACS CT - values must contain no decimal points.

### 2.0.5

#### Enhancements

- BCv14 App - Updated the logic in handling the Remaining Amount in the Direct Debit Split Amount functionality.

- BCv17 App - Updated the logic in handling the Remaining Amount in the Direct Debit Split Amount functionality.

- BCv15 App - Updated the logic in handling the Remaining Amount in the Direct Debit Split Amount functionality.

- BCv14 App - Updated the logic in handling the rounding in the Direct Debit Split Amount functionality. Split Amount was changed to two decimal places.

- BCv17 App - Updated the logic in handling the rounding in the Direct Debit Split Amount functionality. Split Amount was changed to two decimal places.

- BCv15 App - Updated the logic in handling the rounding in the Direct Debit Split Amount functionality. Split Amount was changed to two decimal places.

### 2.0.4

#### Enhancements

- BCv15 App - The default data codeunit was removed from running at App Install and is now surfaced on the SD Interface Banking Setup as standard with our other ISV products.

#### Bug Fixes

- BCv15 App - Created an XMLport for the RBS Statement and added the statement definition to the install pack.

### 2.0.3

#### Enhancements

- BCv15 App - Barclays MT103 - In the Export check codeunit the "Bank code" check was removed.

#### Bug Fixes

- BCv15 App - For the Barclays BACs Credit Transfer a change was made to stamp the Destination Account Name to the Vendor Name.

### 2.0.2

#### Enhancements

- BCv16 App - Objects were renamed to fix AppSource Validation errors.

- BCv16 App - Made a change to the Barclays BACs CT to update the Destination Account Name with the Vendor Name.

- BCv16 App - Made a change to the Barclays MT103 Codeunit to remove the check on the Bank Code. 

- BCv16 App - Warnings in the code were fixed as per AppSource rules.

- BCv16 App - Ulster Bank Statement objects were created.

- BCv16 App - BOI SEPA CT objects were created.

- BCv16 App - BOI SEPA DD objects were created.

- BCv16 App - BOI Statement objects were created.

- BCv16 App - NIB (Danske) SEPA DD objects were created.

- BCv16 App - NIB (Danske) SEPA CT objects were created.

- BCv16 App - NIB (Danske) SEPA CAMT Statement objects were created.

- BCv16 App - A change was made to remove the default data codeunit from running at App Install and instead surface on the SD Interface Banking Setup.

- BCv16 App - Bank Export/import Setup Names were standardized.

- BCv16 App - Reworked the Test Package for this version of the product.

- BCv16 App - The permission set was updated.

- BCv16 App - The translation files were updated.

- BCv16 App - For the Barclays BACS CT file functionality a checkbox flag was added to the Banking Import/Export page to allow users to send Amount with Decimals or without.

- BCv16 App - An Action Caption on Role Centre was changed.

- BCv16 App - BOI SEPA DD format was added to the Install Codeunit.

- BCv16 App - NIB (Danske) SEPA CT format was added to the Install Codeunit.

- BCv16 App - BOI SEPA CT format was added to the Install Codeunit.

- BCv16 App - Bank Export/import Setup Names were standardized.

- BCv16 App - Reworked the Test Package for this version of the product.

- BCv16 App - Caption on the Decimal Indicator on the Banking Import/Export page was updated to Barclays BACS CT Decimal Indicator.

- BCv16 App - Made a change to the Barclays MT103 Codeunit to remove the check on the Bank Code.

- BCv16 App - Made a change to the Barclays BACs CT to update the Destination Account Name with the Vendor Name.


#### Bug Fixes

- BCv15 App - For Barclays SCT MT103 Vendor Name and Address needed to print instead of the the Bank Address.


### 2.0.1

#### Enhancements

- BCv16 App - The caption on the SD Interface Banking Role Centre was updated.

- BCv16 App - The product logo was changed.

- BCv16 App - The Test Codeunits were updated.

- BCv16 App - An integration event for the DD Amount Split functionality was exposed.

- BCv16 App - A change was made to the tag DbtAgt in the Ulster Bank SEPA CT codeunit.

- BCv16 App - A Setup table and Page for the for the Direct Debit Amount Spread functionality was added to the BCv16 code base.

- BCv16 App - A Direct Debit Amount Spread setup Action was added to the SD Interface Banking Role Centre.

- BCv16 App - A Split Amount action was added to the DD Collection Entries page for the Direct Debit Amount Spread functionality.

- BCv16 App - A management codeunit for the Direct Debit Amount Spread functionality was added to the BCv16 code base.

#### Bug Fixes

- BCv16 App - Fixed an issue where the SD Interface Banking activity pages were not showing in the Tell Me in the IE region.

### 2.0.0

#### Enhancements

- BCv14 - An integration event for the DD Amount Split functionality was exposed.

- A change was made to the tag DbtAgt in the Ulster Bank SEPA CT codeunit.

### 1.0.0

#### Enhancements

- BCv15 App - A change was made to the reinstall codeunit logic.

- BCv14 App - A change was made to the reinstall codeunit logic.

- BCv16 App - A change was made to the r-install codeunit logic.

- BCv15 App - The CT Export field in the Payment Methods page was renamed to Credit Transfer.

- BCv14 App - The CT Export field in the Payment Methods page was renamed to Credit Transfer.

- BCv16 App - A change was made to the remove headers in the PT-X DD codeunit.

- BCv15 App - A change was made to the remove headers in the PT-X DD codeunit.

- BCv14 App - A change was made to the remove headers in the PT-X DD codeunit.

- BCv16 App - The CT Export field in the Payment Methods page was renamed to Credit Transfer.

- BCv16 App - A change was made to display SD Interface Banking Activity pages when searching for SD or SDY in the Tell Me.

- BCv16 App - In the PT-X DD file the Direct Debit Reference is now picked up from the Customer Bank Code.

- BCv15 App - In the PT-X DD file the Direct Debit Reference is now picked up from the Customer Bank Code.

- BCv14 App - In the PT-X DD file the Direct Debit Reference is now picked up from the Customer Bank Code.

- BCv16 App - A number of changes were made to the Barclays SEPA CT MT103 file.

- BCv14 App - A number of changes were made to the Barclays SEPA CT MT103 file.

- BCv15 App - A number of changes were made to the Barclays SEPA CT MT103 file.

- BCv14 App - A number of fixes were made to the Barclays BACS CT file.

- BCv15 App - A number of fixes were made to the Barclays BACS CT file.

- BCv16 App - A number of fixes were made to the Barclays BACS CT file.

- BCv15 App - A Setup table and Page for the for the Direct Debit Amount Spread functionality was added to the BCv16 code base.

- BCv15 App - A Direct Debit Amount Spread setup Action was added to the SD Interface Banking Role Centre.

- BCv15 App - A Split Amount action was added to the DD Collection Entries page for the Direct Debit Amount Spread functionality.

- BCv15 App - A management codeunit for the Direct Debit Amount Spread functionality was added to the BCv16 code base.

- BCv14 App - A Direct Debit Amount Spread setup Action was added to the SD Interface Banking Role Centre.

- BCv14 App - A Split Amount action was added to the DD Collection Entries page for the Direct Debit Amount Spread functionality.

- BCv14 App - A management codeunit for the Direct Debit Amount Spread functionality was added to the BCv16 code base.

- BCv14 App - A Setup table and Page for the for the Direct Debit Amount Spread functionality was added to the BCv16 code base.

- BCv16 App - Created Test Codeunits.

- BCv16 App - Updated the tool tips on the Role Center.

- BCv15 App - Report 43015100 was removed from the product as this feature is handled by standard D365BCv15 and above.

- BCv16 App - Removed Report 43015100 SDY INBK Create DD Collection from the build as this feature is now handled by standard Microsoft Dynamics 365BCV15 and above.

- BCv16 App - Objects were readied for submission to App Source.

- BCv16 App - the BCv15 source code was converted to a BCv16 code base.

- A bank format for Barclays MT103 SCT export was created.

- A change was made to allow GBP currency export for the BACS PT-X  DD format.

- On the Payment journal lines, a change was made to the Testfield Currency to allow for Blank (LCY) or GBP.

- Fixes to the Bank Account Code were made to the Barclays BACS export file.

- Fixes were made to the Barclays BACS journal lines check codeunit.

- BCv15 App - the BCv14 code base was converted to a BCv15 code base.

- A codeunit was created to check the journal lines for BACS CT export.

- A Danske (NIB) BACS CT report was created.

- A Role Centre was created for SD Interface Banking.

- A BACS for PT-X CT and DD was created for Coutts Bank.

- A BACS CT output for Barclays Bank was created.

- A Banking Activity Panel with KPIs was created for SD Interface Banking.

- A Danske (NIB) BACS CT report was created.

- Ulster Bank SEPA DD objects were created.

- Ulster Bank SEPA CT objects were created.

- AIB SEPA Statement objects were created.

- AIB SEPA DD objects were created.

- AIB SEPA CT objects were created.

#### Bug Fixes

- BCv14 App - An issue was fixed where the amount didn't split on the DD Collection if one of the lines isn't a split payment terms code line.

- Fixes were made to the BACs PT-X DD format.

