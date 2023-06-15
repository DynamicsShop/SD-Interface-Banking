## SD Interface Banking Releases

### 3.0.1

#### Enhancements

- BCv14 App - A number of small fixes for H2H Connectivity were made.

### 3.0.0

#### Enhancements

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

