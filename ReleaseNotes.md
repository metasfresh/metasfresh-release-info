# About this document

This file contains the tasks/issues which we implement in metasfresh, in a chronological fashion (latest first).

Additional notes:
 * The metasfresh source code is hosted at https://github.com/metasfresh/metasfresh
 * The metasfresh website is at [metasfresh.com/en](https://metasfresh.com/en) (English), [metasfresh.com](https://metasfresh.com/) (German)
 * You can also follow us on Twitter: [@metasfresh](https://twitter.com/metasfresh) (English), [@metasfreshDE](https://twitter.com/metasfreshde) (German D/A/CH)

Here come the actual release notes:

# metasfresh 5.177 (upcoming RC)

## Features
* metasfresh
 * [#17108](https://github.com/metasfresh/metasfresh/pull/17108) Add index for better perf if there are many unprocessed workpackages
 * [#17096](https://github.com/metasfresh/metasfresh/issues/17096) Error when deleting production orders or changing products in po
 * [#17099](https://github.com/metasfresh/metasfresh/issues/17099) Product maturing - 1 - tables and configs
 * [#17088](https://github.com/metasfresh/metasfresh/issues/17088) Bewegungsdatum shall be current date in shipment
 * [#17066](https://github.com/metasfresh/metasfresh/issues/17066) Port the fix for PP_Product_Bom_Recursive to release
 * [#17015](https://github.com/metasfresh/metasfresh/pull/17015) Introduce AD_Process.FilenamePattern
 * [#17047](https://github.com/metasfresh/metasfresh/pull/17047) Printing Store-To-Disk - Add option to include AD_PInstance_ID in PDF filename
 * [#17011](https://github.com/metasfresh/metasfresh/issues/17011) CSV-Process - Add option Remove quotes from Export CSV File header and lines
 * [#16954](https://github.com/metasfresh/metasfresh/pull/16954) Add new column Fully delivered or invoiced in C_Order
 * [#16902](https://github.com/metasfresh/metasfresh/pull/16902) Change REST API /hu/bySerialNo to return HUs with any status
 * [#16944](https://github.com/metasfresh/metasfresh/pull/16944) Dynamic output of Mac addresses in REST API
 * [#16968](https://github.com/metasfresh/metasfresh/pull/16968) MobileUI - Change CU Qty of a TU
 * [#16993](https://github.com/metasfresh/metasfresh/pull/16993) Sort login roles by caption but keep system administrator as last
 * [#16786](https://github.com/metasfresh/metasfresh/pull/16786) Dunning changes: copy poReference from source document, and allow using it (and the document prefix) as document number for the dunning document
 * [#16976](https://github.com/metasfresh/metasfresh/pull/16976) FE Inline filter: fix caret which jumps to the end after each key pressed
 * [#16972](https://github.com/metasfresh/metasfresh/pull/16972) FE Fix inline filter for the case when the parameters are empty
 * [#16979](https://github.com/metasfresh/metasfresh/pull/16979) FE Fix included Tab shall load on changes
 * [#16960](https://github.com/metasfresh/metasfresh/pull/16960) windowHandler.js reducer: preserve layout.activeTab when updating the layout 
 * [#16964](https://github.com/metasfresh/metasfresh/issues/16964) Warehouse in Shipment Disposition as search field  
 * [#16949](https://github.com/metasfresh/metasfresh/issues/16949) Compute order tax for the date promised
 * [#16898](https://github.com/metasfresh/metasfresh/issues/16898) MobileUI move HU to LU and support bulk scan
 * [#16791](https://github.com/metasfresh/metasfresh/issues/16791) Zählbestand Reihenfolge is not transferred to Material Cockpit  
 * [#16873](https://github.com/metasfresh/metasfresh/issues/16873) Product planning data is being ignored when manufacturing orders are generated automatically
 * [#16807](https://github.com/metasfresh/metasfresh/issues/16807) Adjustment window Auftrag
 * [#16794](https://github.com/metasfresh/metasfresh/pull/16794) Fix not working cache invalidation on source column changed
 * [#16866](https://github.com/metasfresh/metasfresh/pull/16866) intensive care uat fixCacheInvalidationOnSourceColumnChange 2
 * [#16779](https://github.com/metasfresh/metasfresh/pull/16779) MobileUI - TargetWeight rounding, ignore non stocked components 
 * [#16802](https://github.com/metasfresh/metasfresh/pull/16802) MobileUI - Unload Funnel (Save Funnel weight) 
 * [#16830](https://github.com/metasfresh/metasfresh/pull/16830) Set Discontinued and Discontinued From columns as filters in the Produkt window
 * [#16815](https://github.com/metasfresh/metasfresh/pull/16815) modular contract settings unique index
 * [#16789](https://github.com/metasfresh/metasfresh/pull/16789) DocumentCollection: on cache invalidate don't remove Document from cache if it's new and not already saved
 * [#16816](https://github.com/metasfresh/metasfresh/issues/16816) Extend lookup widget to 20 entries 
 * [#16769](https://github.com/metasfresh/metasfresh/issues/16769) ic114 - EDI - Add Quantities in price-UOM to DESADV-Pack-Item 
 * [#16772](https://github.com/metasfresh/metasfresh/pull/16772) Sys Config webui.frontend.view.showCommentsMarker
 * [#16742](https://github.com/metasfresh/metasfresh/pull/16742) Move PLU File config to product
 * [#16743](https://github.com/metasfresh/metasfresh/pull/16743) Excel output for cost prices report
 * [#16644](https://github.com/metasfresh/metasfresh/pull/16644) mobile UI mfg - Configure to be able to pre-print QR codes
 * [#16551](https://github.com/metasfresh/metasfresh/pull/16551) Distribute cucumber-tests over more runners
 * [#16625](https://github.com/metasfresh/metasfresh/pull/16625) Cache API improvements for observability (REST API) and configuration
 * [#16688](https://github.com/metasfresh/metasfresh/issues/16688) Missing translation in Shipment Disposition
 * [#16660](https://github.com/metasfresh/metasfresh/issues/16660) ICs not created
 * [#16609](https://github.com/metasfresh/metasfresh/issues/16609) Create Price list report for all business partners on a key date
 * [#16629](https://github.com/metasfresh/metasfresh/issues/16629) mobile UI - HU manager: button to associate Leich+Mehl QR lot number to the HU QR Code of paloxe
 * [#16628](https://github.com/metasfresh/metasfresh/issues/16628) mobile UI picking: When scanning a Leich+Mehl QR code we have to split out a TU from the palette
 * [#16619](https://github.com/metasfresh/metasfresh/issues/16619) Deactivating of prices for discontinued products not working 
 * [#16617](https://github.com/metasfresh/metasfresh/pull/16617)
   Printing - support different number of copies based on location
 * [#16524](https://github.com/metasfresh/metasfresh/issues/16524) API endpoint add greeting
 * [#16574](https://github.com/metasfresh/metasfresh/issues/16574) Automatic update of contract periods based on checkbox shipping address and billing address 
 * [#16558](https://github.com/metasfresh/metasfresh/issues/16558) Use the price precision in jasper reports
 * [#16564](https://github.com/metasfresh/metasfresh/issues/16564) When picking, filter for the warehouse of the currently assigned workplace 
 * [#16550](https://github.com/metasfresh/metasfresh/pull/16550) removed C_DocType.CompletedNotification_BoilerPlate_ID column. Added AD_Org.Name as docOutbound mail context variable
 * [#16545](https://github.com/metasfresh/metasfresh/issues/16545) Creating unique-constraints with User friendly ErrorMsg not working anymore 
 * [#16534](https://github.com/metasfresh/metasfresh/issues/16534) Use harvest calendar for modular and interim payment contracts
 * [#16516](https://github.com/metasfresh/metasfresh/issues/16516) Add Max Lot Size override in Manufacturing Candidate
 * [#16514](https://github.com/metasfresh/metasfresh/pull/16514) Switch to new DHL API
 * [#16484](https://github.com/metasfresh/metasfresh/issues/16484) Serial Number Production Automation - Implementation
 * [#16510](https://github.com/metasfresh/metasfresh/issues/16510) Include crop year & crop calendar in Purchase Order
 * [#16496](https://github.com/metasfresh/metasfresh/issues/16496) Cleanup HU(-label) related processes
 * [#16471](https://github.com/metasfresh/metasfresh/issues/16471) Introduce Mobile UI Picking Profile
 * [#16456](https://github.com/metasfresh/metasfresh/pull/16456) Process to receive additional HUs
 * [#16457](https://github.com/metasfresh/metasfresh/issues/16457) Remove jasper-process Picking Slot Label (Jasper)
 * [#16451](https://github.com/metasfresh/metasfresh/issues/16451) Feature to hide AD_Client_ID/AD_Org_ID from all windows
 * [#16446](https://github.com/metasfresh/metasfresh/issues/16446) Mobile UI - Include Product Value in Issue Raw Materials
 * [#16435](https://github.com/metasfresh/metasfresh/issues/16435) Mobile UI - Manufacturing orders are not sorted by sequence
 * [#16430](https://github.com/metasfresh/metasfresh/pull/16430) Products Proposal modal update
 * [#16355](https://github.com/metasfresh/metasfresh/pull/16355) Modular Contract Log improvements 
 * [#16340](https://github.com/metasfresh/metasfresh/pull/16340) Implementing Shipping Notification-> Modular Contract Log
 * [#16351](https://github.com/metasfresh/metasfresh/pull/16351) Allow using marketing campaigns from * org
 * [#16328](https://github.com/metasfresh/metasfresh/issues/16328) New My Approvals window
 * [#16306](https://github.com/metasfresh/metasfresh/issues/16306) Add Missing Translations
 * [#16281](https://github.com/metasfresh/metasfresh/issues/16281) Picking&Packing - add a posibility to prohibit the mix of HUs for different orders
 * [#16294](https://github.com/metasfresh/metasfresh/issues/16294) Modular contract log: customization and corrections
 * [#16284](https://github.com/metasfresh/metasfresh/issues/16284) Add the column "Invoicing Group" in the modular contract log
 * [#16279](https://github.com/metasfresh/metasfresh/pull/16279) Delete Erntekalender calendar
 * [#16181](https://github.com/metasfresh/metasfresh/issues/16181) SAP accounting journal gross invoice
 * [#16258](https://github.com/metasfresh/metasfresh/issues/16258) Sales Order -> Modular Contract Log (Sales)
 * [#16236](https://github.com/metasfresh/metasfresh/pull/16236) Shopware - Allow OLCand-Processing to be configurable
 * [#16239](https://github.com/metasfresh/metasfresh/pull/16239) Interim Invoice Log
 * [#16230](https://github.com/metasfresh/metasfresh/issues/16230) Add reltype shipment schedule to shipping notification
 * [#16196](https://github.com/metasfresh/metasfresh/issues/16196) Interim Invoice - Cucumber
 * [#16197](https://github.com/metasfresh/metasfresh/pull/16197) Sales Bidding Invoice
 * [#16191](https://github.com/metasfresh/metasfresh/pull/16191) DESADV CU-Quantities in case of TU-UOMs
 * [#16175](https://github.com/metasfresh/metasfresh/issues/16175) Subtask 3 (Vertragsbausteinlog Caching & Co) - Recreate logs
 * [#16180](https://github.com/metasfresh/metasfresh/issues/16180) Vertragsbausteinlog Caching & Co - Cucumber
 * [#16177](https://github.com/metasfresh/metasfresh/issues/16177) Sales Modular Contract and log  
 * [#16189](https://github.com/metasfresh/metasfresh/pull/16189) Credit Memo shall have no payment slip
 * [#16171](https://github.com/metasfresh/metasfresh/pull/16171) Add C_BPartner_InterimContract_GenerateInterimInvoice process
 * [#16158](https://github.com/metasfresh/metasfresh/issues/16158) Import products from excel
 * [#16150](https://github.com/metasfresh/metasfresh/issues/16150) Urproduzent Ableitung IPS nach metasfresh
 * [#16139](https://github.com/metasfresh/metasfresh/pull/16139) New columns in M_HU_Trace_Excel
 * [#16134](https://github.com/metasfresh/metasfresh/pull/16134) Add Open Sans Fonts
 * [#16116](https://github.com/metasfresh/metasfresh/issues/16116) Modular contract logs for manufacturing: Positive/negative quantity for receipt/issue (resp.)
 * [#16129](https://github.com/metasfresh/metasfresh/issues/16129) Adjustment business partner grid view and name search problem
 * [#16118](https://github.com/metasfresh/metasfresh/issues/16118) Subtask 2 (Vertragsbausteinlog Caching & Co) - Async processing
 * [#16115] (https://github.com/metasfresh/metasfresh/pull/16115) Manufacturing: Issue any product
 * [#16100](https://github.com/metasfresh/metasfresh/issues/16100) Vertragsbaustein Log - Export for editing
 * [#16097](https://github.com/metasfresh/metasfresh/pull/16097) Interim Contract Log / Interim ReceiptLine Log
 * [#16063](https://github.com/metasfresh/metasfresh/issues/16063) Sales Invoice -> Modular Contract Log
 * [#16082](https://github.com/metasfresh/metasfresh/issues/16082) VA-Auftrag IST-Start, IST-Start/ Ende after simulation complete CO
 * [#16072](https://github.com/metasfresh/metasfresh/issues/16072) Add Interim Invoiceable Status to Receipt 
 * [#16065](https://github.com/metasfresh/metasfresh/pull/16065) (Vertragsbausteinlog Caching & Co) - Performance enhancements #16065
 * [#16062](https://github.com/metasfresh/metasfresh/pull/16062) Create Interim Invoice
 * [#16059](https://github.com/metasfresh/metasfresh/issues/16059) New tables ModCntr_InvoicingGroup and ModCntr_InvoicingGroup_Product 
 * [#16027](https://github.com/metasfresh/metasfresh/issues/16027) SubTask 1 (Debitoren Rechnung -> Vertragsbaustein Log) - adding fields in files
 * [#16040](https://github.com/metasfresh/metasfresh/issues/16040) Introduce ModCntr_Log.ContractType
 * [#16052](https://github.com/metasfresh/metasfresh/issues/16052) Product search (filter) - name
 * [#16032](https://github.com/metasfresh/metasfresh/issues/16032) Sammelstellen/ Verladeorte/ Annahmestellen
 * [#16026](https://github.com/metasfresh/metasfresh/pull/16026) C_BPartner_Interim table and column corrections 
 * [#16001](https://github.com/metasfresh/metasfresh/pull/16001) SubTask 1 (Kreditoren Rechnung (Vorfinanzierung) -> Vertragsbaustein Log) - Create C_BPartner_InterimContract
 * [#16013](https://github.com/metasfresh/metasfresh/pull/16013) Improve DESADV matching with BPartnerId
 * [#15980](https://github.com/metasfresh/metasfresh/issues/15980) local currency conversion needs to look at tax departure country
 * [#15992](https://github.com/metasfresh/metasfresh/issues/15992) Cloning of workflows 
 * [#15951](https://github.com/metasfresh/metasfresh/pull/15951) SAP GL Journal: Implement Reverse Charge VAT support
 * [#15959](https://github.com/metasfresh/metasfresh/issues/15959) Do not apply warehouse link to cost materials (product type: service) 
 * [#15938](https://github.com/metasfresh/metasfresh/issues/15938) [CR058] Closed status for PO/SO  
 * [#15919](https://github.com/metasfresh/metasfresh/pull/15919) getc_period_id_by_date function 
 * [#15957](https://github.com/metasfresh/metasfresh/issues/15957) Import Bank Accounts 
 * [#15964](https://github.com/metasfresh/metasfresh/pull/15964) External System Printing Client
 * [#15907](https://github.com/metasfresh/metasfresh/issues/15907) Order -> Contract Module Log 
 * [#15843](https://github.com/metasfresh/metasfresh/pull/15843) Include VHUs reserved for an orderline into available stock, for ShipmentSchedule purposes
 * [#15943](https://github.com/metasfresh/metasfresh/issues/15943) Produktion -> Vertragsbaustein Log 
 * [#15941](https://github.com/metasfresh/metasfresh/pull/15941) Support several QR Labels
 * [#15860](https://github.com/metasfresh/metasfresh/pull/15860) Add support for document completed boilerplate notification
 * [#15894](https://github.com/metasfresh/metasfresh/issues/15894) [CR070] Link material to warehouse 
 * [#15855](https://github.com/metasfresh/metasfresh/pull/15855) bPartner api generate location name on update if set to null
 * [#15848](https://github.com/metasfresh/metasfresh/issues/15848) Modular Contract: PO Cucumber
 * [#15842](https://github.com/metasfresh/metasfresh/pull/15842) Modular Contract: Receipt
 * [#15879](https://github.com/metasfresh/metasfresh/pull/15879) Create request for source org on bPartner org change
## Fixes
* metasfresh
* [#16740](https://github.com/metasfresh/metasfresh/pull/16740) Support at least 6 digist in the QR Code

# metasfresh 5.176 (current RC)
## Features
* metasfresh
  * [#15910](https://github.com/metasfresh/metasfresh/issues/15910) Validate contract terms for modular contracts
  * [#15897](https://github.com/metasfresh/metasfresh/issues/15897) (Bestellung -> Vertragsbaustein Log) - Overview and test the entire feature -> fixes
  * [#15864](https://github.com/metasfresh/metasfresh/issues/15863) Open Items (managed) window
  * [#15863](https://github.com/metasfresh/metasfresh/issues/15863) Cancelling FEC need to be possible
  * [#15861](https://github.com/metasfresh/metasfresh/issues/15861) Hauptbuch Journal Anpassung Beschreibung 
  * [#15805](https://github.com/metasfresh/metasfresh/pull/15805) DeliveryPlanningICHandlerExtension: ActLoadDate from Planning docs with no instructions
  * [#15804](https://github.com/metasfresh/metasfresh/pull/15804) ShipmentScheduleFromSubscriptionOrderLineVetoer: fix veto logic
  * [#15819](https://github.com/metasfresh/metasfresh/issues/15819) (Inventur -> Vertragsbaustein Log) - Inventory -> contract module log
  * [#15783](https://github.com/metasfresh/metasfresh/issues/15783) Create contracts from PO and other operations related to it
  * [#15807](https://github.com/metasfresh/metasfresh/issues/15784) (Bestellung -> Vertragsbaustein Log) - Add related document links
  * [#15784](https://github.com/metasfresh/metasfresh/issues/15784) (Bestellung -> Vertragsbaustein Log) - Create contact module log when PO happens
  * [#15671](https://github.com/metasfresh/metasfresh/pull/15671) Vertragsbausteinlog Factory
  * [#15765](https://github.com/metasfresh/metasfresh/pull/15765) Window Bestellanforderung
  * [#15736](https://github.com/metasfresh/metasfresh/issues/15736) Serverabsturz am 2023-06-22
  * [#15715](https://github.com/metasfresh/metasfresh/issues/15715) (Bestellung -> Vertragsbaustein Log) - Missing Fields and structures
  * [#15670](https://github.com/metasfresh/metasfresh/issues/15670) Include DESADV-Documentnumber(s) in INVOIC  
  * [#15689](https://github.com/metasfresh/metasfresh/pull/15689) Module Contract tables and columns renaming
  * [#15611](https://github.com/metasfresh/metasfresh/issues/15611) New Flag in c_bpartner `isManual` and Import Format for Business Partner 
  * [#15663](https://github.com/metasfresh/metasfresh/issues/15662) Dunning windows - set IsBetaFunctionality=NO
  * [#15690](https://github.com/metasfresh/metasfresh/issues/15690) Add/ Prepare language it_IT as systemlanguage
  * [#15672](https://github.com/metasfresh/metasfresh/issues/15672) Housekeeping references - Iteration 3
  * [#15576](https://github.com/metasfresh/metasfresh/issues/15576) [Purchase_housekeeping 2] reference additional documents
  * [#15626](https://github.com/metasfresh/metasfresh/pull/15668) Extend BPartner Import
  * [#15653](https://github.com/metasfresh/metasfresh/issues/15653) Datefields in InvoiceCandidates
  * [#15610](https://github.com/metasfresh/metasfresh/pull/15610) Make sure to update the Updated column when propagating TRL update to base table
  * [#15545](https://github.com/metasfresh/metasfresh/issues/15545) [Purchase_housekeeping 1] Purchase order
  * [#15626](https://github.com/metasfresh/metasfresh/pull/15626) Limit Generate Goods Issue by Shipment Disposition On Hand
  * [#15623](https://github.com/metasfresh/metasfresh/issues/15623) Stacktrace when IBAN via Endpoint is not correct
  * [#15549](https://github.com/metasfresh/metasfresh/issues/15549) New window: Vertragsbaustein Log (Contract Module Log)
  * [#15509](https://github.com/metasfresh/metasfresh/issues/15509) New window: Baustein Typ (Contract Module Type)
  * [#15574](https://github.com/metasfresh/metasfresh/pull/15574) Aktionspreis: Add UOM to Aktionspreise subtab in Product>>Aktionspreise
  * [#15569](https://github.com/metasfresh/metasfresh/pull/15569) Add message for the order credit limit info notification
  * [#15533](https://github.com/metasfresh/metasfresh/pull/15533) Order Based Credit Limit shall not prevent order creation and completion
  * [#15543](https://github.com/metasfresh/metasfresh/pull/15543) [Sales_housekeeping 6] Delivery planning Change Logic of additional lines process
  * [#15528](https://github.com/metasfresh/metasfresh/issues/15528) [Sales_housekeeping 4] Allocating FEC
  * [#15563](https://github.com/metasfresh/metasfresh/pull/15563) Change date format to `dd.mm.yyyy` for Invoice Candidate Import
  * [#15554](https://github.com/metasfresh/metasfresh/pull/15554) Improve performance of de_metas_endcustomer_fresh_reports.Docs_Sales_Dunning_QR_Code()
  * [#15440](https://github.com/metasfresh/metasfresh/pull/15440) Add and propagate user element strings from order to invoice
  * [#15447](https://github.com/metasfresh/metasfresh/issues/15447) New Process: Add access to menu recursively for a Role
  * [#15516](https://github.com/metasfresh/metasfresh/issues/15516) Dunning Mails to seperate Mail address
  * [#15530](https://github.com/metasfresh/metasfresh/issues/15530) Bank Statement Import: Migros Bank camt53
  * [#15481](https://github.com/metasfresh/metasfresh/issues/15481) Campaign prices: fill out fields - follow up
  * [#15519](https://github.com/metasfresh/metasfresh/issues/15519) Make 'New Record' option configurable at AD_Field level
  * [#15476](https://github.com/metasfresh/metasfresh/issues/15476) Invoice candidate import: Take out billto contact ID as mandatory field
  * [#15484](https://github.com/metasfresh/metasfresh/issues/15484) Contract term window customization
  * [#15489](https://github.com/metasfresh/metasfresh/issues/15489) Payment allocation modal: action to allocate credit memo/ invoice.
  * [#15471](https://github.com/metasfresh/metasfresh/issues/15471) Add TaxCode to Accounting Transaction Details Window
  * [#15473](https://github.com/metasfresh/metasfresh/issues/15473) Show the default Invoice identifier in ESR Payment Import window ID - 540159
  * [#15452](https://github.com/metasfresh/metasfresh/issues/15452) Fix Materialcockpit displaying 404
  * [#15427](https://github.com/metasfresh/metasfresh/issues/15427) Make "MD_Cockpit / MD_Candidate" related tests unflaky
  * [#15155](https://github.com/metasfresh/metasfresh/issues/15155) Material Disposition: Lot for Lot 
  * [#15406](https://github.com/metasfresh/metasfresh/pull/15406) Don't try to update M_Product.LowLevel when cloning PP_Product_BOMs.
  * [#15399](https://github.com/metasfresh/metasfresh/issues/15399) Modernize developers' docker-compose.yml
  * [#15375](https://github.com/metasfresh/metasfresh/issues/15375) Use correct currency in dunning mail 
  * [#15329](https://github.com/metasfresh/metasfresh/issues/15329) Add to Marketing Campaign from Partner Export window
  * [#15343](https://github.com/metasfresh/metasfresh/issues/15343) Fix Calendar Remaining Translations
  * [#15331](https://github.com/metasfresh/metasfresh/issues/15331) B2b: Kommisionierung rückgängig machen
  * [#15260](https://github.com/metasfresh/metasfresh/issues/15260) SAP FI interface: GL entries to be NOT interfaced into SAP
  * [#15319](https://github.com/metasfresh/metasfresh/issues/15319) FollowUp: Server Error Message Zahllauf 
  * [#15147](https://github.com/metasfresh/metasfresh/issues/15147) RAA Datenaustausch Wareneingang Prüfling
  * [#15272](https://github.com/metasfresh/metasfresh/issues/15272) External project reference Sequence changes
  * [#15221](https://github.com/metasfresh/metasfresh/issues/15221) People resource reservation master data
  * [#15154](https://github.com/metasfresh/metasfresh/issues/15154) DESADV ist fehlerhaft - Lieferscheinnummer anstelle von DESADV Nummer übertragen
  * [#15100](https://github.com/metasfresh/metasfresh/issues/15100) Handle multiple SalesRep in invoices
  * [#15133](https://github.com/metasfresh/metasfresh/issues/15133) SAP FI interface: export Assignment
  * [#15090](https://github.com/metasfresh/metasfresh/issues/15090) [IEUIF003] SAP business partner interface: MC and storage partners
  * [#15095](https://github.com/metasfresh/metasfresh/issues/15095) When creating a Counter Doc for C_Order, take into account the HandOver informations
  * [#15049](https://github.com/metasfresh/metasfresh/issues/15049) Tax Reporting: Local currency conversion
  * [#15075](https://github.com/metasfresh/metasfresh/issues/15075) Add support for invoice reviews
  * [#15074](https://github.com/metasfresh/metasfresh/issues/15074) [IEUE043] GL journal (SAP) cannot be reversed
  * [#15063](https://github.com/metasfresh/metasfresh/issues/15063) SAP Interface UOM Mapping
  * [#15046](https://github.com/metasfresh/metasfresh/issues/15046) CR042 mbank (Poland bank data) - AC4 
  * [#14971](https://github.com/metasfresh/metasfresh/issues/14971) Interface - Transfer Bio Label
  * [#15013](https://github.com/metasfresh/metasfresh/issues/15013) Adding new process Offene Posten (Excel)
  * [#15007](https://github.com/metasfresh/metasfresh/issues/15007) Receipt fact accounts in document currency
  * [#14856](https://github.com/metasfresh/metasfresh/issues/14856) Update to Java 17
  * [#14954](https://github.com/metasfresh/metasfresh/issues/14954) Check if the Source HU already exist before trying to add a new one
  * [#14951](https://github.com/metasfresh/metasfresh/issues/14951) Add section code to Inventory, Bank Statement & Movement
  * [#14762](https://github.com/metasfresh/metasfresh/issues/14762) RAA Datenaustausch: Soll-Start/Ende Prüfschritt - Follow-Up 01
  * [#14831](https://github.com/metasfresh/metasfresh/issues/14831) Stücklistenexport nach Excel - Lieferant mit ausgeben
  * [#14826](https://github.com/metasfresh/metasfresh/issues/14826) Stücklistenexport nach Excel - Reihenfolge der Zeilen wird ignoriert
  * [#14879](https://github.com/metasfresh/metasfresh/issues/14879) Fix the Open Linked Accounting transactions action
  * [#14722](https://github.com/metasfresh/metasfresh/issues/14722) Report Accounts information changes
  * [#14835](https://github.com/metasfresh/metasfresh/issues/14835) Manage filtering with attributes in HU reservation screen
  * [#14841](https://github.com/metasfresh/metasfresh/issues/14841) SAP GL Journal Window Adjustment
  * [#14849](https://github.com/metasfresh/metasfresh/pull/14849) Allow creation of goods issue for the qty that ws just received in the case of b2b
  * [#14813](https://github.com/metasfresh/metasfresh/issues/14813) Resource reservation presentation 
  * [#14755](https://github.com/metasfresh/metasfresh/issues/14755) Correction Invoices 
  * [#14709](https://github.com/metasfresh/metasfresh/issues/14709) CR042 mbank (Poland bank data) 
  * [#14721](https://github.com/metasfresh/metasfresh/issues/14721) Partner Block and Release - TSV format 
  * [#14768](https://github.com/metasfresh/metasfresh/issues/14768) InvoiceEnqueueing considers already processed invoice candidates and is therefore slow
  * [#14686](https://github.com/metasfresh/metasfresh/issues/14686) Do not reset `BillToAddress` whenever Delivery Address changed
  * [#14714](https://github.com/metasfresh/metasfresh/issues/14714) Enable filter search on Locator when moving HU
  * [#14706](https://github.com/metasfresh/metasfresh/issues/14706) Import Shopware Product Variants  
  * [#14683](https://github.com/metasfresh/metasfresh/issues/14683) Partner Block and Release 
  * [#14645](https://github.com/metasfresh/metasfresh/issues/14645) Order Window Ivict adaptions (Billto Default, Drop Shipment)
  * [#14649](https://github.com/metasfresh/metasfresh/issues/14649) country-based doctype sequences
  * [#14672](https://github.com/metasfresh/metasfresh/issues/14672) Sort by serial number 
  * [#14663](https://github.com/metasfresh/metasfresh/issues/14663) Prevent changing account schema currency if there are current costs in that currency
  * [#14448](https://github.com/metasfresh/metasfresh/issues/14448) product notice not translated on PO
  * [#14652](https://github.com/metasfresh/metasfresh/issues/14652) Import Data File with C_Activity
  * [#14632](https://github.com/metasfresh/metasfresh/issues/14632) Add C_Invoice_Candidate.ActualLoadingDate and populate from earliest M_ShipperTransportation 
  * [#14542](https://github.com/metasfresh/metasfresh/issues/14542) When importing inventory, different CUs that are in the same TU get summed up incorrectly
  * [#14596](https://github.com/metasfresh/metasfresh/issues/14596) SAP Partner ID in Business Partner location is set to null after credit limit import
  * [#14537](https://github.com/metasfresh/metasfresh/issues/14537) Moving Average Invoice Costing Method
  * [#14582](https://github.com/metasfresh/metasfresh/issues/14582) Hus in zur Prüfung können in Produktion benutzt werden 
  * [#14521](https://github.com/metasfresh/metasfresh/issues/14521) Delivery Instruction Cucumber Tests
  * [#14554](https://github.com/metasfresh/metasfresh/issues/14554) Add accountConceptualName to fact_acct 
  * [#14569](https://github.com/metasfresh/metasfresh/issues/14569) Generate Invoice with Allowing Override Due Date
  * [#14467](https://github.com/metasfresh/metasfresh/issues/14467) Import Exchange Rate from .dat file
  * [#14520](https://github.com/metasfresh/metasfresh/issues/14520) Avoid useless updates to AD_Field_Trl
  * [#14538](https://github.com/metasfresh/metasfresh/issues/14538) Field Renaming Delivery Planning Window
  * [#14508](https://github.com/metasfresh/metasfresh/issues/14508) Create Cucumber for accounting 
  * [#14492](https://github.com/metasfresh/metasfresh/issues/14492) Delivery Planning - Shortage and Overage
  * [#14500](https://github.com/metasfresh/metasfresh/issues/14500) Credit Limit - Reporting
  * [#14470](https://github.com/metasfresh/metasfresh/issues/14470) Inventory management: Add Process To Move CUQY To another Location
  * [#14475](https://github.com/metasfresh/metasfresh/issues/14475) Fix /invoices/payment 
  * [#14408](https://github.com/metasfresh/metasfresh/issues/14408) Delivery Based Credit Limit 
  * [#14469](https://github.com/metasfresh/metasfresh/issues/14469) SAP: mark only imported fields as read-only
  * [#14477](https://github.com/metasfresh/metasfresh/issues/14477) Drop stepDef `all the hu data is reset` 
  * [#14446](https://github.com/metasfresh/metasfresh/issues/14446) Order dispo shall show complete transaction 
  * [#14458](https://github.com/metasfresh/metasfresh/issues/14458) Implement invoice API
  * [#14444](https://github.com/metasfresh/metasfresh/issues/14444) Delivery Planning - Delivery Instructions Amendment
  * [#14235](https://github.com/metasfresh/metasfresh/issues/14235) Enhance REST-API with cache control
  * [#14402](https://github.com/metasfresh/metasfresh/issues/14402) ExternalSys-Other: Send Address MF to ES (=> C__BPartner_Location) 
  * [#14437](https://github.com/metasfresh/metasfresh/issues/14437) Allow setting manual tax rate for PO lines created via SO to PO process
  * [#14210](https://github.com/metasfresh/metasfresh/issues/14210) ExternalSys-Other: Send project info from MF to ES - Part II (=> C_Project.ExternalId) 
  * [#14104](https://github.com/metasfresh/metasfresh/issues/14104) ExternalSys-Other: Send project info from MF to ES (=>C_Project_WO_Step data) 
  * [#14377](https://github.com/metasfresh/metasfresh/issues/14377) group invoices and credit memos into a single document 
  * [#14370](https://github.com/metasfresh/metasfresh/pull/14370) import Allergens for bom products
  * [#14429](https://github.com/metasfresh/metasfresh/pull/14429)  Increased Credit Limit be decreased again
  * [#14433](https://github.com/metasfresh/metasfresh/pull/14433)  Add M_SectionCode_ID to C_BPartner_Stats
  * [#14354](https://github.com/metasfresh/metasfresh/issues/14354) Automatically update PP Orders when a new BOM Version is imported
  * [#14414](https://github.com/metasfresh/metasfresh/issues/14414) Add Department Data Structures
  * [#14368](https://github.com/metasfresh/metasfresh/issues/14368) Enhancements SAP import product
  * [#14362](https://github.com/metasfresh/metasfresh/issues/14362) Enhancements SAP import BPartner
  * [#14215](https://github.com/metasfresh/metasfresh/issues/14215) Delivery Instruction 
  * [#14233](https://github.com/metasfresh/metasfresh/issues/14233) Add additional translation sync
  * [#14245](https://github.com/metasfresh/metasfresh/issues/14245) Use pagination when exchanging data with CMS-platform
  * [#14201](https://github.com/metasfresh/metasfresh/issues/14201) Allow lotNo to be set automatically, based on sequence Number
  * [#14160](https://github.com/metasfresh/metasfresh/issues/14160) SAP: Make sure credit limits are automatically enforced after import 
  * [#14223](https://github.com/metasfresh/metasfresh/issues/14223) Enhance import BOM Formula from GRS
  * [#14217](https://github.com/metasfresh/metasfresh/issues/14217) Show weight Diff on scale by sending target weight (Soehnle)
  * [#14155](https://github.com/metasfresh/metasfresh/issues/14155) Fixing de_DE and de_CH Translations
  * [#14199](https://github.com/metasfresh/metasfresh/issues/14199) Product API bpartnerProductItems update fails 
  * [#14156](https://github.com/metasfresh/metasfresh/issues/14156) Create Interface to upload contacts to Active Campaign 
  * [#14165](https://github.com/metasfresh/metasfresh/issues/14165) Gantt: New Prüfaufträge shall always be simulation initially 
  * [#14164](https://github.com/metasfresh/metasfresh/issues/14164) New Accounting Dimensions: Section Code and Order
  * [#14092](https://github.com/metasfresh/metasfresh/issues/14092) Allow EDI-Invoice without order-id
  * [#14159](https://github.com/metasfresh/metasfresh/issues/14159) Extend Export Accounting
  * [#14122](https://github.com/metasfresh/metasfresh/issues/14122) Add new picking-process 
  * [#14038](https://github.com/metasfresh/metasfresh/issues/14038) Get WorkOrder Projects from API  
  * [#14135](https://github.com/metasfresh/metasfresh/issues/14135) Support 4 parent levels in Balance Sheet 
  * [#14105](https://github.com/metasfresh/metasfresh/issues/14105) Sub-Task No 5: Test & Fix Sales order (w/ ship ) - Product Planning - Distribution 
  * [#14103](https://github.com/metasfresh/metasfresh/issues/14103) Delivery Planning: Open and Close processes 
  * [#14108](https://github.com/metasfresh/metasfresh/pull/14108) Don't validate ASI for unique attributes in service repair PP_Orders
  * [#14090](https://github.com/metasfresh/metasfresh/issues/14090) update build to postgres 15.1
  * [#14096](https://github.com/metasfresh/metasfresh/pull/14096) Delete delivery plannings on inout schedule deletion 
  * [#13430](https://github.com/metasfresh/metasfresh/issues/13430) github & everhour - Services Invoicing
  * [#14050](https://github.com/metasfresh/metasfresh/issues/14050) Delivery planning: New qty columns
  * [#14011](https://github.com/metasfresh/metasfresh/issues/14011) Sub-Task No 4: Test & Fix Inventory interaction with MD_Cockpit 
  * [#14060](https://github.com/metasfresh/metasfresh/issues/14060) Format Qty based on on the precision defined in SysConfig
  * [#13953](https://github.com/metasfresh/metasfresh/pull/13953) [SAP]: Add mappings for required masterdata
  * [#13980](https://github.com/metasfresh/metasfresh/pull/13980) Introduce C_BPartner_Location.VATaxID
  * [#14032](https://github.com/metasfresh/metasfresh/pull/14032) webui: (refreshViewOnChangeEvents) notify FE also when we have pure rows removal
  * [#14023](https://github.com/metasfresh/metasfresh/pull/14023) webui: Make sure all views are notified on view addition changes
  * [#14017](https://github.com/metasfresh/metasfresh/pull/14017) webui: When rows are changed consider also adding new ones to the view if it's matching the filter
  * [#13604](https://github.com/metasfresh/metasfresh/issues/13604) Add ExternalHeaderId to invoiceCand header aggregation key
  * [#13561](https://github.com/metasfresh/metasfresh/issues/13561) Approval for invoicing: add description to field and process
  * [#13631](https://github.com/metasfresh/metasfresh/issues/13631) InEffect invoice candidates testId
  * [#13942](https://github.com/metasfresh/metasfresh/issues/13942) Delivery Planning
  * [#13998](https://github.com/metasfresh/metasfresh/issues/13998) Sub-Task No 3: Test & Fix Purchase candidate interaction with MD_Cockpit
  * [#13937](https://github.com/metasfresh/metasfresh/issues/13937) Add source sub configs for ExternalSystem_Config_SAP 
  * [#13979](https://github.com/metasfresh/metasfresh/pull/13979) External system config metasfresh improvement 
  * [#13955](https://github.com/metasfresh/metasfresh/pull/13955) ExternalSystem component for batched bpartner-upserts via REST follow up 
  * [#13929](https://github.com/metasfresh/metasfresh/issues/13929) ExternalSystem component for batched bpartner-upserts via REST
  * [#13251](https://github.com/metasfresh/metasfresh/pull/13251) Resolve importing of product variants from Shopware
  * [#13970](https://github.com/metasfresh/metasfresh/issues/13970) Externally referenced records: further improvements 
  * [#13968](https://github.com/metasfresh/metasfresh/issues/13968) Include in MD_Stock inactive HUs
  * [#13962](https://github.com/metasfresh/metasfresh/pull/13962) Extend BPartner API with Credit Limit
  * [#13959](https://github.com/metasfresh/metasfresh/issues/13959) GL Journal Update Totals
  * [#13819](https://github.com/metasfresh/metasfresh/issues/13819) Import BPartner mastedata from SAP
  * [#13921](https://github.com/metasfresh/metasfresh/issues/13921) Make Invoice Candidate read only if referenced on open invoices 
  * [#13746](https://github.com/metasfresh/metasfresh/issues/13746) Micrometer Performance Monitoring
  * [#13885](https://github.com/metasfresh/metasfresh/issues/13885) Follow-Up - Produktionsdisposition - Iteration 1 - Creating PP Order by machine size
  * [#13948](https://github.com/metasfresh/metasfresh/pull/13948) Swing Login: show only System role 
  * [#13947](https://github.com/metasfresh/metasfresh/pull/13947) Manufacturing Order - Weighing Run (part 2)
  * [#13920](https://github.com/metasfresh/metasfresh/pull/13920) Manufacturing Order - Weighing Run
  * [#13838](https://github.com/metasfresh/metasfresh/pull/13838) The excel export process should consider the latest BOM version and exclude the oldest version with validto date 
  * [#13825](https://github.com/metasfresh/metasfresh/pull/13825) The excel export process should consider the latest BOM version
  * [#13824](https://github.com/metasfresh/metasfresh/issues/13824) Fix BOM Recursive Report
  * [#13811](https://github.com/metasfresh/metasfresh/pull/13811) Fix github actions failures
  * [#13946](https://github.com/metasfresh/metasfresh/pull/13946) mobile UI: mfg: Show allergens
  * [#13935](https://github.com/metasfresh/metasfresh/pull/13935) mobile UI - mfg: Show Hazard Symbols
  * [#13913](https://github.com/metasfresh/metasfresh/pull/13913) Fix Manufacturing Candidates layout
  * [#13933](https://github.com/metasfresh/metasfresh/pull/13933) Doc_GLJournal: consider GL_JournalLine.GL_JournalLine_Group when grouping into FactTrxLines
  * [#13936](https://github.com/metasfresh/metasfresh/pull/13936) mobile UI: Barcode text input: debounce
  * [#13846](https://github.com/metasfresh/metasfresh/pull/13846) Start Order and New Partner from Partner Window
  * [#13797](https://github.com/metasfresh/metasfresh/pull/13797) ProcessExecutionResult.webuiNewRecord support | Create New Sales Order from BPartner window processes java code 
  * [#13594](https://github.com/metasfresh/metasfresh/issues/13594) Search Wizard enters wrong partner in C_BPartner_SalesRep_ID
  * [#13922](https://github.com/metasfresh/metasfresh/issues/13922) Make UOM key on product import not case sensitive 
  * [#13904](https://github.com/metasfresh/metasfresh/issues/13904) Create translations for base language also for non AD_Element tables
  * [#13912](https://github.com/metasfresh/metasfresh/pull/13912) CallExternalSystemActivityHandler: persist last scanned QR Code
  * [#13883](https://github.com/metasfresh/metasfresh/pull/13883) mobile UI: manufacturing: Call to External System activity 
  * [#13767](https://github.com/metasfresh/metasfresh/pull/13767) Exclude Reversed Invoices from Open Items Report
  * [#13908](https://github.com/metasfresh/metasfresh/pull/13908) mobile UI: display issue/receipt/coproduct icons
  * [#13766](https://github.com/metasfresh/metasfresh/issues/13766) Exclude Reversed Invoices from Open Items Report 
  * [#13881](https://github.com/metasfresh/metasfresh/pull/13881) Manufacturing candidate window: compute some totals for selected rows
  * [#13841](https://github.com/metasfresh/metasfresh/pull/13841) HU Clearance: Status Test Pending (Json) 
  * [#13829](https://github.com/metasfresh/metasfresh/issues/13829) Test&Fix MD_Cockpit_DocumentDetail 
  * [#13844](https://github.com/metasfresh/metasfresh/issues/13844) IEUE045.U01 Incoming payment management - Follow-Up 01 
  * [#13845](https://github.com/metasfresh/metasfresh/issues/13845) BUG: Grant discount twice during allocate payment process
  * [#13850](https://github.com/metasfresh/metasfresh/issues/13850) Unique Attributes Implementation
  * [#13784](https://github.com/metasfresh/metasfresh/issues/13784) Price difference from offer to order(Add IsKeepProposalPrices)
  * [#13854](https://github.com/metasfresh/metasfresh/pull/13854) Set incoterms from partners only if has a value
  * [#13857](https://github.com/metasfresh/metasfresh/pull/13857) webui: (re)evaluate document field readonly and display logic based on user's role
  * [#13855](https://github.com/metasfresh/metasfresh/pull/13855) Tax window: fix field names
  * [#13801](https://github.com/metasfresh/metasfresh/issues/13801) Add IsAlwaysUpdatable and ReadOnlyLogic to AD_Field 
  * [#13822](https://github.com/metasfresh/metasfresh/issues/13822) Add fields for Sales 
  * [#13840](https://github.com/metasfresh/metasfresh/issues/13840) Add support for Soehenle scales
  * [#13831](https://github.com/metasfresh/metasfresh/issues/13831) [Cucumber] Import file - identify account by IBAN
  * [#13833](https://github.com/metasfresh/metasfresh/issues/13833) Add Role_Group to role window and context
  * [#13805](https://github.com/metasfresh/metasfresh/pull/13805) Fix github actions failures
  * [#13813](https://github.com/metasfresh/metasfresh/issues/13813) InvoiceCandidate - Allow creating invoices with DocStatus=IP
  * [#13812](https://github.com/metasfresh/metasfresh/issues/13812) HU Clearance status: Test Pending
  * [#13778](https://github.com/metasfresh/metasfresh/issues/13778) Externally referenced records: show ReadOnly reason in UI
  * [#13745](https://github.com/metasfresh/metasfresh/issues/13745) Import material (product) data from SAP
  * [#13685](https://github.com/metasfresh/metasfresh/issues/13685) Allow externally maintained records to be read-only in metasfresh
  * [#13758](https://github.com/metasfresh/metasfresh/issues/13758) IEUE045.U01 Incoming payment management
  * [#13685](https://github.com/metasfresh/metasfresh/issues/13685) Allow externally maintained records to be read-only in metasfresh 
  * [#13755](https://github.com/metasfresh/metasfresh/issues/13755) Look up C_OLcand.M_HU_PI_Item_Product_ID also via StoreGLN
  * [#13772](https://github.com/metasfresh/metasfresh/issues/13772) Set "-" in MAC Address instead of null 
  * [#13717](https://github.com/metasfresh/metasfresh/issues/13717) Sub-Task No 2: Test & Fix Sales order (w/ ship ) - ProductPlanning - Manufacturing 
  * [#13751](https://github.com/metasfresh/metasfresh/issues/13751) Renumber C_OLCand.Line when sending from excel to metasfresh
  * [#13651](https://github.com/metasfresh/metasfresh/issues/13651) Allow invoking "Other" ExternalSystem via API
  * [#13740](https://github.com/metasfresh/metasfresh/issues/13740) Fix inventory move line
  * [#13716](https://github.com/metasfresh/metasfresh/issues/13716) Creating PP Order by machine size
  * [#13733](https://github.com/metasfresh/metasfresh/issues/13733) edit translations for ad_references #13733
  * [#13707](https://github.com/metasfresh/metasfresh/issues/13707) Fix Mail notifications
  * [#13648](https://github.com/metasfresh/metasfresh/issues/13648) Propagate Section_ID from OLCand to Payment
  * [#13646](https://github.com/metasfresh/metasfresh/issues/13646) Cucumber: EffortControl coverage
  * [#13663](https://github.com/metasfresh/metasfresh/issues/13663) Sub-Task No 1: Test & Fix Sales/Purchase order (w/ ship & receive) - No Product Planning 
  * [#13643] https://github.com/metasfresh/metasfresh/pull/13643#pullrequestreview-1118261799 Support SEPA for QR
  * [#13649](https://github.com/metasfresh/metasfresh/issues/13649) Allow product configuration to lock HUs for that product that are received or manufactured
  * [#13623](https://github.com/metasfresh/metasfresh/issues/13623) New Contracts do not work on with startdate on the end of the month
  * [#13625](https://github.com/metasfresh/metasfresh/issues/13625) Material-Cockpit Add C_Order QtyReserved column
  * [#13580](https://github.com/metasfresh/metasfresh/issues/13580) IC Handle the case of respective record going "into limbo"
  * [#13603](https://github.com/metasfresh/metasfresh/issues/13603) Disallow reactivating/reverting documents that have ICs approved for invoicing
  * [#13614](https://github.com/metasfresh/metasfresh/issues/13614) Desadv Packs - in depth testing (camel & cucumber)
  * [#13589](https://github.com/metasfresh/metasfresh/issues/13589) Fix Basepricelist retrieval vor product proposal without save
  * [#13571](https://github.com/metasfresh/metasfresh/issues/13571) M_AttributeUse.MandatoryForManufacturing
  * [#13558](https://github.com/metasfresh/metasfresh/issues/13558) Improve "update dunning candidate" process 
  * [#13578](https://github.com/metasfresh/metasfresh/issues/13578) When creating a counter doc C_Order, take into account the dropship information
  * [#13541](https://github.com/metasfresh/metasfresh/issues/13541) Unify de.metas.project.workorder && de.metas.project.workorder.data
  * [#13144](https://github.com/metasfresh/metasfresh/issues/13144) Create Test harness for mobileUI's API
  * [#13509](https://github.com/metasfresh/metasfresh/issues/13509) Generic importer for invoice candidates
  * [#13423](https://github.com/metasfresh/metasfresh/issues/13423) Partial payment overview (aka Interim Invoice): the proces
  * [#13466](https://github.com/metasfresh/metasfresh/issues/13466) Purchase call orders 
  * [#13458](https://github.com/metasfresh/metasfresh/issues/13458) Load Budget Project JSONs into metasfresh
  * [#13431](https://github.com/metasfresh/metasfresh/pull/13431) Set-up Github webhooks for syncing issues 
  * [#13442](https://github.com/metasfresh/metasfresh/issues/13442) Option to set the base language if same as the previous one #13442
  * [#13443](https://github.com/metasfresh/metasfresh/issues/13443) Workorder-Project - Inherit certain properties from parent
  * [#13405](https://github.com/metasfresh/metasfresh/issues/13405) Allow custom columns in API upserts (for Budget-Project)
  * [#13415](https://github.com/metasfresh/metasfresh/issues/13415) Customer returns error
  * [#13413](https://github.com/metasfresh/metasfresh/issues/13413) Display project fields in various windows(SO, Shipment, Request(all)...)
  * [#13392](https://github.com/metasfresh/metasfresh/issues/13316) Extend invoice-candidate test-coverage to IC QtyToInoviceOverride
  * [#13392](https://github.com/metasfresh/metasfresh/issues/13392) Final Product Costprice S2: lines creation process 
  * [#13384](https://github.com/metasfresh/metasfresh/issues/13384) Tests and Error Message for SEPA Export with QR IBAN
  * [#13368](https://github.com/metasfresh/metasfresh/issues/13368) Partial Payment Invoicing S4: Invoice candidate 
  * [#13364](https://github.com/metasfresh/metasfresh/issues/13364) Available for sale - trigger recomputation when shipment schedule is closed/reopened + shopware sync when config changes
  * [#13323](https://github.com/metasfresh/metasfresh/issues/13323) Partial Payment Invoicing: flatrate conditions
  * [#13339](https://github.com/metasfresh/metasfresh/issues/13339) Final Product Costprice S1: tables and window
  * [#13354](https://github.com/metasfresh/metasfresh/issues/13354) Accounting Transactions sidelist Reference for documents missing again 
  * [#13337](https://github.com/metasfresh/metasfresh/issues/13337) Adjustment Payment/Bank Statement Windows
  * [#13338](https://github.com/metasfresh/metasfresh/issues/13338) Support QR IBAN in SEPA export 
  * [#13280](https://github.com/metasfresh/metasfresh/issues/13280) Revolut Export Fixes
  * [#13308](https://github.com/metasfresh/metasfresh/issues/13308) Partial Payment Invoicing: prepare warehouse and prefinancing settings
  * [#13302](https://github.com/metasfresh/metasfresh/issues/13302) Change base language via Process
  * [#13314](https://github.com/metasfresh/metasfresh/issues/13314) Prevent price lookup from base PLV
  * [#13296](https://github.com/metasfresh/metasfresh/issues/13296) Support additional shopware payment type
  * [#13283](https://github.com/metasfresh/metasfresh/issues/13283) Create REST Endpoints to read and write WorkOrder- and Budget-C_Projects
  * [#13282](https://github.com/metasfresh/metasfresh/issues/13282) OLCand => Order Extend test-coverage cover bill-, dropship- and handover-partners
  * [#13277](https://github.com/metasfresh/metasfresh/issues/13277) Sys config: address and user to update when creating an invoice
  * [#13223](https://github.com/metasfresh/metasfresh/issues/13223) Leich&Mehl Part II
  * [#13246](https://github.com/metasfresh/metasfresh/issues/13246) Record sql  "raise warning" output in AD_PInstanceLog
  * [#13227](https://github.com/metasfresh/metasfresh/issues/13227) Picking QA Step
  * [#13242](https://github.com/metasfresh/metasfresh/pull/13242) build metasfresh via dockerbuilds
  * [#13255](https://github.com/metasfresh/metasfresh/issues/13255) Add source infos to account sheet report 
  * [#13162](https://github.com/metasfresh/metasfresh/issues/13162) Available for sales qty from metasfresh to shopware
  * [#13176](https://github.com/metasfresh/metasfresh/pull/13176) assert_period_open: improve error reporting when document was not found
  * [#13175](https://github.com/metasfresh/metasfresh/pull/13175) fact_acct_summary_partial_from_date_functions
  * [#13192](https://github.com/metasfresh/metasfresh/issues/13192) Port stepdefs and implement material-receipt cucumber tests 
  * [#13178](https://github.com/metasfresh/metasfresh/issues/13178) Gebindekonfiguration not set in PP_Order from PP_Order Dispo although set in sales orderline
  * [#13183](https://github.com/metasfresh/metasfresh/issues/13183) Rename Sektion to Organisation
  * [#13154](https://github.com/metasfresh/metasfresh/issues/13154) Shopware - implement getBPartners action 
  * [#13148](https://github.com/metasfresh/metasfresh/issues/13148) Datenaustausch - Provide default Title for invoice document
  * [#13158](https://github.com/metasfresh/metasfresh/issues/13158) Adjust Window Manufacturing Candidate
  * [#13153](https://github.com/metasfresh/metasfresh/issues/13153) Add FirmenbuchNR to Business Partner Window
  * [#13132](https://github.com/metasfresh/metasfresh/issues/13132) Customizing: Add fr_CH Language as System Language
  * [#13062](https://github.com/metasfresh/metasfresh/issues/13062) Pricing issue 
  * [#13107](https://github.com/metasfresh/metasfresh/issues/13107) KPI - Add sum of SO/PO orders today / of last 7 days
  * [#13084](https://github.com/metasfresh/metasfresh/issues/13084) Create REST Endpoint to read and write C_Projects
  * [#12938](https://github.com/metasfresh/metasfresh/issues/12938) Shopware - set pricing system on created business partners
  * [#12824](https://github.com/metasfresh/metasfresh/issues/12824) Clarify and document externalsystems multithreading behavior
  * [#13054](https://github.com/metasfresh/metasfresh/issues/13054) Optimize `Fresh_Account_Info_Report` 
  * [#13074](https://github.com/metasfresh/metasfresh/issues/13074) externalsystems - document timestamp-usage
  * [#13017](https://github.com/metasfresh/metasfresh/issues/13017) EDI - Extend INVOIC export format
  * [#13038](https://github.com/metasfresh/metasfresh/issues/13038) Campaign price where m_pricingsystem_id is set not used in orderline
  * [#12931](https://github.com/metasfresh/metasfresh/issues/12931) API - Export PP_Orders with extended informations
  * [#12982](https://github.com/metasfresh/metasfresh/issues/12982) Korrektur action in material receipt candidates is not considered correctly in Material Dispo
  * [#12999](https://github.com/metasfresh/metasfresh/issues/12999) Allow Defining Tax-Categories without a M_ProductPrice
  * [#12974](https://github.com/metasfresh/metasfresh/issues/12974) Default paymentrule for packing item causes >1 invoice for the same order
  * [#13016](https://github.com/metasfresh/metasfresh/issues/13016) Shopware Fix order-item/bundle-sorting - part deux
  * [#13024](https://github.com/metasfresh/metasfresh/issues/13024) Improve API-Errormessage on wrong Headers
  * [#12966](https://github.com/metasfresh/metasfresh/issues/12966) Improve ways of API request troubleshooting
  * [#12964](https://github.com/metasfresh/metasfresh/issues/12964) Support purchase candidates with same product and diffente ASI in one PO
  * [#12928](https://github.com/metasfresh/metasfresh/issues/12928) shopware - use pagination when polling for orders
  * [#12849](https://github.com/metasfresh/metasfresh/issues/12849) Handle multiple contacts and negative amounts in invoices
  * [#12919](https://github.com/metasfresh/metasfresh/pull/12919) Annotate cucumber scenarios with unique test case Ids
  * [#12826](https://github.com/metasfresh/metasfresh/issues/12826) MetasfreshEventBusService - always post events to rabbitMQ
  * [#12840](https://github.com/metasfresh/metasfresh/issues/12840) Overhaul C_OLcand => C_Order processing
  * [#12837](https://github.com/metasfresh/metasfresh/issues/12837) Shopware Fix order-item/bundle-sorting
  * [#13045](https://github.com/metasfresh/metasfresh/pull/13045) log to loggables why an attribute based price is not applied

## Fixes
* metasfresh
  * [#15751](https://github.com/metasfresh/metasfresh/pull/15751) Fix FTS type error
  * [#15752](https://github.com/metasfresh/metasfresh/pull/15752) update lucene dependency version to match elasticsearch
  * [#15698](https://github.com/metasfresh/metasfresh/issues/15698) BUG: C_Project_ID gets overwritten when propagated to shipment line
  * [#15490](https://github.com/metasfresh/metasfresh/issues/15490) Payment Allocation action bug
  * [#14980](https://github.com/metasfresh/metasfresh/issues/14980) Override Due Date should be filled with the invoice due date
  * [#14915](https://github.com/metasfresh/metasfresh/issues/14915) Fix missing columns in GridView
  * [#14803](https://github.com/metasfresh/metasfresh/issues/14803) Accounting Issues - Invalid accounting operation structure
  * [#14686](https://github.com/metasfresh/metasfresh/issues/14686) Do not reset BillToAddress whenever Delivery Address changed
  * [#14700](https://github.com/metasfresh/metasfresh/issues/14700) Delivery Planning Generate Goods Issue without stock should not be possible
  * [#14651](https://github.com/metasfresh/metasfresh/issues/14651) Solve on-prem ExternalSys-Other-API problems  
  * [#14381](https://github.com/metasfresh/metasfresh/issues/14381) Set C_doctypeTarget_ID as filter in C_Order
  * [#14366](https://github.com/metasfresh/metasfresh/pull/14366) POInfoColumn.ValueMin, ValueMax: trim blank to null
  * [#14346](https://github.com/metasfresh/metasfresh/issues/14346) Propagate `POReference` from PO to MR
  * [#14187](https://github.com/metasfresh/metasfresh/issues/14187) update infrastructure db dockerfile to work with new images
  * [#13546](https://github.com/metasfresh/metasfresh/issues/13546) DATEV Export Performance Problem 
  * [#14095](https://github.com/metasfresh/metasfresh/pull/14095#pullrequestreview-1215114428) Sum amounts per vatcode
  * [#14019](https://github.com/metasfresh/metasfresh/issues/14019) [BUG] BPartnerRestController v2: path orgCode param is not consolidated with the request body
  * [#14072](https://github.com/metasfresh/metasfresh/issues/14072) Fix Sales Order - void selected order with related documents
  * [#14036](https://github.com/metasfresh/metasfresh/issues/14036) remove remaining oids from tables
  * [#14003](https://github.com/metasfresh/metasfresh/pull/14003) Fix NPE that happens if IExportProcessor.process throws an exception
  * [#14027](https://github.com/metasfresh/metasfresh/issues/14027) Display SEPA/REVOLUT Export Details
  * [#13906](https://github.com/metasfresh/metasfresh/pull/13906) Delete chat when deleting documents and implement voiding draft orders
  * [#13884](https://github.com/metasfresh/metasfresh/pull/13884) fix jenkins - also allow skipping cucumber tests
  * [#13723](https://github.com/metasfresh/metasfresh/pull/13723) Fix Other tag
  * [#13868](https://github.com/metasfresh/metasfresh/issues/13868) [Cucumber] Fix cucumber tests failing due to Daylight saving time
  * [#13753](https://github.com/metasfresh/metasfresh/issues/13753) Adjust auto-vacuum settings on translation tables
  * [#13725](https://github.com/metasfresh/metasfresh/issues/13725) C_DocTypeShipment_ID not respected when generating Receipt/Shipment
  * [#13586](https://github.com/metasfresh/metasfresh/issues/13586) Fix material-dispo bug
  * [#13533](https://github.com/metasfresh/metasfresh/issues/13533) BUG: I_C_InvoiceCandidate.QtyDelivered wrongly computed for manual invoice candidates 
  * [#13550](https://github.com/metasfresh/metasfresh/issues/13550) [React] - Calendar gives blank screen when selecting a date from past
  * [#13487](https://github.com/metasfresh/metasfresh/issues/13487) [React] - Infinite loop for /dropdown call
  * [#13535](https://github.com/metasfresh/metasfresh/issues/13535) Extend Order's Product-Proposal - Fix Bug
  * [#13261](https://github.com/metasfresh/metasfresh/issues/13261) AvailableForSales to Shopware - Fix terminology
  * [#13286](https://github.com/metasfresh/metasfresh/issues/13286) Display document validation message
  * [#13257](https://github.com/metasfresh/metasfresh/pull/13257) available for sales stock fix
  * [#13215](https://github.com/metasfresh/metasfresh/issues/13215) Description and documentnote are not copied from doctype into shipment
  * [#13218](https://github.com/metasfresh/metasfresh/pull/13218) Show Adr attribute details
  * [#13201](https://github.com/metasfresh/metasfresh/pull/13201) add new accounts in Deckungsbeitragsrechnung 
  * [#13204](https://github.com/metasfresh/metasfresh/pull/13204) fix flaky test: Create sales order with different ASI, on complete no production candidate is found
  * [#13197](https://github.com/metasfresh/metasfresh/pull/13197) cucumber fixes
  * [#13170](https://github.com/metasfresh/metasfresh/pull/13170) hotfix RV_UnPosted: DateTrx was used instead of DateAcct for M_MatchInv and M_MatchPO
  * [#13169](https://github.com/metasfresh/metasfresh/pull/13169) db functions: getC_Calendar_ID, getC_Period_ID_by_Date 
  * [#13179](https://github.com/metasfresh/metasfresh/issues/13179) Count QtyDelivered as zero if all inouts are reveserd 
  * [#13112](https://github.com/metasfresh/metasfresh/issues/13112) Fix Zoom Across HU Editor
  * [#13105](https://github.com/metasfresh/metasfresh/issues/13104) Exclude Password Reset process from DebugMailTo
  * [#13086](https://github.com/metasfresh/metasfresh/issues/13086) Windows adjustments & fixing Trls 
  * [#13046](https://github.com/metasfresh/metasfresh/issues/13046) Fix DatePicker format in custom windows
  * [#13062](https://github.com/metasfresh/metasfresh/issues/13062) Pricing issue
  * [#13043](https://github.com/metasfresh/metasfresh/issues/13043) Fix disabled unit tests from `de.metas.manufacturing`
  * [#12997](https://github.com/metasfresh/metasfresh/issues/12997) Open amt incorrect after vendor credit memo is created for a vendor invoice
  * [#12980](https://github.com/metasfresh/metasfresh/issues/12980) Scale Price not used despite usescaleprice=S
  * [#12991](https://github.com/metasfresh/metasfresh/issues/12991) For Picking Profile "Group by Order" the order and bpartner are not displayed in Picking Terminal
  * [#13001](https://github.com/metasfresh/metasfresh/issues/13001) Error on customer return 
  * [#12978](https://github.com/metasfresh/metasfresh/issues/12978) Respect UOM precision when calculating package weights
  * [#12986](https://github.com/metasfresh/metasfresh/issues/12986) Password displayed when hovering over the *** with mouse, w/o using the eye icon 
  * [#12919](https://github.com/metasfresh/metasfresh/pull/12925) fix flaky 'exportExternalReferenceToRabbitMQ.feature' scenario #12925

# metasfresh 5.175
## Features
* metasfresh
  * [#13789](https://github.com/metasfresh/metasfresh/issues/13789) Investigate github actions failures 
  * [#13637](https://github.com/metasfresh/metasfresh/issues/13637) Cucumber: drop MD_Stock_StepDef#truncateMDStockData
  * [#13376](https://github.com/metasfresh/metasfresh/issues/13376) Cucumber: Products (item) invoice candidates
  * [#13355](https://github.com/metasfresh/metasfresh/issues/13355) Packing material invoice candidates: shipments
  * [#13449](https://github.com/metasfresh/metasfresh/issues/13449) Empties Receive and Returns
  * [#13395](https://github.com/metasfresh/metasfresh/issues/13395) Packing material invoice candidates: receipts
  * [#13198](https://github.com/metasfresh/metasfresh/issues/13198) Tell camel which auth token to use when connecting to MF
  * [#13041](https://github.com/metasfresh/metasfresh/issues/13041) Create cucumber-harness for invoice and payment allocation
  * [#12760](https://github.com/metasfresh/metasfresh/issues/12760) Create import/export for C_Campaign_price
  * [#13456](https://github.com/metasfresh/metasfresh/issues/13456) Delivery Rules & Delivery Fifo #13456
  * [#13464](https://github.com/metasfresh/metasfresh/issues/13464) Tax calculation for orders where C_Bpartner_Location != Dropship Location (and AD_Org’s Bpartner Location country != Dropship Location country)
  * [#13448](https://github.com/metasfresh/metasfresh/issues/13448) Address on invoice is the latest billto location from bpartner
  * [#7151](https://github.com/metasfresh/metasfresh/issues/7151) On page switching (in parent view) the includedView for the selected parent row needs to be refreshed
  * [#10032](https://github.com/metasfresh/metasfresh/issues/10032) Cleanup table styles
  * [#11732](https://github.com/metasfresh/metasfresh/issues/11732) webui frontend: improve how the 502 error is displayed to user 
  * [#11740](https://github.com/metasfresh/metasfresh/issues/11740) Implement overdelivery in Manufacturing order picking
  * [#11871](https://github.com/metasfresh/metasfresh/issues/11871) M_AttributeUse mandatory
  * [#11900](https://github.com/metasfresh/metasfresh/issues/11900) Alberta - Get new Patient-API field(s)
  * [#11905](https://github.com/metasfresh/metasfresh/issues/11905) Receive BOM master data from GRS
  * [#11914](https://github.com/metasfresh/metasfresh/issues/11914) Automatically invoice order with flatrate term for new partner
  * [#11919](https://github.com/metasfresh/metasfresh/issues/11919) Fetch layout on attributes PATCH request
  * [#11943](https://github.com/metasfresh/metasfresh/issues/11943) Production dispo
  * [#11944](https://github.com/metasfresh/metasfresh/issues/11944) Create GRS mapping docu
  * [#11945](https://github.com/metasfresh/metasfresh/issues/11945) Replace v1.BPRelationRouteBuilder with a v2 pendant
  * [#11947](https://github.com/metasfresh/metasfresh/issues/11947) Automatic Shipping and Invoicing - async batch overhaul
  * [#11955](https://github.com/metasfresh/metasfresh/issues/11955) Fixes around sales-order => purchase-order
  * [#11961](https://github.com/metasfresh/metasfresh/issues/11961) Ability to link sales invoices to purchase invoices
  * [#11962](https://github.com/metasfresh/metasfresh/issues/11962) Nachbelastung aus Kreditorenseite
  * [#11968](https://github.com/metasfresh/metasfresh/issues/11968) Implement possibility to know easily the first contract from a hierarchy chain
  * [#11969](https://github.com/metasfresh/metasfresh/issues/11969) Introduce C_BPartner.PO_InvoiceRule
  * [#11985](https://github.com/metasfresh/metasfresh/issues/11985) Add POReference to C_PurchaseCandidate
  * [#11986](https://github.com/metasfresh/metasfresh/issues/11986) Implement AutodetectDefaultDateFilter
  * [#11991](https://github.com/metasfresh/metasfresh/issues/11991) Send BPartners metasfresh to GRS
  * [#11993](https://github.com/metasfresh/metasfresh/issues/11993) shopware6 - Make product lookup mode configurable
  * [#11995](https://github.com/metasfresh/metasfresh/issues/11995) User does not have access to make OrgChanges
  * [#12000](https://github.com/metasfresh/metasfresh/issues/12000) Extend Bpartner attribute tables
  * [#12007](https://github.com/metasfresh/metasfresh/issues/12007) Credit memo commission instance
  * [#12013](https://github.com/metasfresh/metasfresh/issues/12013) Extend inconterms
  * [#12018](https://github.com/metasfresh/metasfresh/issues/12018) Improve API Audit error response
  * [#12032](https://github.com/metasfresh/metasfresh/issues/12032) Display Problems in material cockpit 
  * [#12035](https://github.com/metasfresh/metasfresh/issues/12035) Cypress tests - end of Nov 2021
  * [#12039](https://github.com/metasfresh/metasfresh/issues/12039) Suppport tags CON and BR_GR, BR_NAME in same time in address capture sequence
  * [#12049](https://github.com/metasfresh/metasfresh/issues/12049) Adding new attributes fields to product window
  * [#12051](https://github.com/metasfresh/metasfresh/issues/12051) On Manufacturing Order, allow printing of only selected HUs
  * [#12059](https://github.com/metasfresh/metasfresh/issues/12059) New columns in BPartner Quick Input
  * [#12066](https://github.com/metasfresh/metasfresh/issues/12066) add `C_User_Role.IsCustomUserRestriction` column
  * [#12070](https://github.com/metasfresh/metasfresh/issues/12070) Create a new window `Additives`
  * [#12071](https://github.com/metasfresh/metasfresh/issues/12071) Sync bpartners using RabbitMQ when changes are made to `C_User_Role` and `C_User_Assigned_Role`
  * [#12079](https://github.com/metasfresh/metasfresh/issues/12079) Enable external system status reporting and control
  * [#12084](https://github.com/metasfresh/metasfresh/issues/12084) When inserting/removing pauses, refresh `C_SubscriptionProgress`
  * [#12086](https://github.com/metasfresh/metasfresh/issues/12086) Save binary data in migration scripts
  * [#12089](https://github.com/metasfresh/metasfresh/issues/12089) Adding nutritional data in product window
  * [#12090](https://github.com/metasfresh/metasfresh/issues/12090) webui frontend: Unfriendly error when you type space in menu search 
  * [#12094](https://github.com/metasfresh/metasfresh/issues/12094) Send M_Product.DicontinuedFrom to Alberta
  * [#12096](https://github.com/metasfresh/metasfresh/issues/12096) Commission Calculation for license fees
  * [#12108](https://github.com/metasfresh/metasfresh/issues/12108) Add m_product_ID to aggregation group for Bestellkontrolle zum Kunden drucken report
  * [#12111](https://github.com/metasfresh/metasfresh/issues/12111) Use Partner name and greeting when rendering address only if there is greeting set
  * [#12113](https://github.com/metasfresh/metasfresh/issues/12113) Support different bpartner-properties in shopware-orders
  * [#12114](https://github.com/metasfresh/metasfresh/issues/12114) Add IsPrintWhenPackingMaterial flag in Product
  * [#12122](https://github.com/metasfresh/metasfresh/issues/12122) Api Audit: `bypass` & `wrap` options
  * [#12125](https://github.com/metasfresh/metasfresh/issues/12125) Include invoice POReference in Payment selection line and SEPA export
  * [#12127](https://github.com/metasfresh/metasfresh/issues/12127) Import product with scale prices
  * [#12128](https://github.com/metasfresh/metasfresh/issues/12128) Overhaul address & contact sync from Shopware6 to metasfresh
  * [#12138](https://github.com/metasfresh/metasfresh/issues/12138) [Frontend] Current page is lost when user redirected to login screen after backed is restarted (on Connection Lost)
  * [#12143](https://github.com/metasfresh/metasfresh/issues/12143) Assign an address to a contact
  * [#12144](https://github.com/metasfresh/metasfresh/issues/12144) Switch other-metasfresh sync to all v2 API
  * [#12149](https://github.com/metasfresh/metasfresh/issues/12149) Extend import product 
  * [#12157](https://github.com/metasfresh/metasfresh/issues/12157) C_BPartner_Location_QuickInput
  * [#12160](https://github.com/metasfresh/metasfresh/issues/12160) Custom filters without parameters are not displayed
  * [#12161](https://github.com/metasfresh/metasfresh/issues/12161) Send BPartners to GRS automatically
  * [#12165](https://github.com/metasfresh/metasfresh/issues/12165) "Connection problem" info when user is already logged in in other tab
  * [#12168](https://github.com/metasfresh/metasfresh/issues/12168) webui frontend: pressing HOME and END in a text field is not showing the carret
  * [#12172](https://github.com/metasfresh/metasfresh/issues/12172) Add a  relation type that points to service projects from sales  order window
  * [#12174](https://github.com/metasfresh/metasfresh/issues/12174) Fix open issues in invoice tax verification feature
  * [#12180](https://github.com/metasfresh/metasfresh/issues/12180) Support BPartner SalesRep in Search assistant
  * [#12182](https://github.com/metasfresh/metasfresh/issues/12182) Adding new column `Long Text Description` to M_Product
  * [#12184](https://github.com/metasfresh/metasfresh/issues/12184) Changing the DE translation of the element IsDropShip
  * [#12185](https://github.com/metasfresh/metasfresh/issues/12185) Support for v4.5 datenaustausch  xml schema
  * [#12192](https://github.com/metasfresh/metasfresh/issues/12192) Logging for camel externalsystems
  * [#12195](https://github.com/metasfresh/metasfresh/issues/12195) Tweak Auto-Send Vendors to GRS
  * [#12200](https://github.com/metasfresh/metasfresh/issues/12200) Create and Export AD_User.Email2 and EMail3
  * [#12202](https://github.com/metasfresh/metasfresh/issues/12202) Maintaine address name
  * [#12206](https://github.com/metasfresh/metasfresh/issues/12206) Focus first filter field whenopening filter panel
  * [#12207](https://github.com/metasfresh/metasfresh/issues/12207) Add indices for better invoicing-perf
  * [#12210](https://github.com/metasfresh/metasfresh/issues/12210) Add parameter `spreadsheetFormat` to `ExportToSpreadsheetProcess`
  * [#12218](https://github.com/metasfresh/metasfresh/issues/12218) Update de-metas-camel-shopware6/README.md
  * [#12221](https://github.com/metasfresh/metasfresh/issues/12221) Automate invoicing and printing the invoices
  * [#12222](https://github.com/metasfresh/metasfresh/issues/12222) Propagate `C_OLCand.ExternalHeaderId` & `C_OLCand.ExternalLineId` to `C_Invoice_Candidate`
  * [#12230](https://github.com/metasfresh/metasfresh/issues/12230) Marketing Contacts created for a large selection of partners
  * [#12234](https://github.com/metasfresh/metasfresh/issues/12234) Include features in inventory position counting
  * [#12237](https://github.com/metasfresh/metasfresh/issues/12237) Add an action to scheduler so that we can start and stop them from the webui
  * [#12239](https://github.com/metasfresh/metasfresh/issues/12239) Add new `exportdate` and `exportby` colums in table `DatevAcctExport`
  * [#12241](https://github.com/metasfresh/metasfresh/issues/12241) Enhance `CheckProcessedAsynBatchWorkpackageProcessor`
  * [#12244](https://github.com/metasfresh/metasfresh/issues/12244) Translated label field contents should respect current user language
  * [#12247](https://github.com/metasfresh/metasfresh/issues/12247) webui frontend: upgrade babel + webpack
  * [#12254](https://github.com/metasfresh/metasfresh/issues/12254) cypress e2e beginning of Jan 2022
  * [#12258](https://github.com/metasfresh/metasfresh/issues/12258) Improve performance of IC creation when extending contracts
  * [#12264](https://github.com/metasfresh/metasfresh/issues/12264) mobile UI: update packages to latest versions / fix vulnerabilities
  * [#12278](https://github.com/metasfresh/metasfresh/issues/12278) Show delivery address on customs invoice if there are several shiopments
  * [#12282](https://github.com/metasfresh/metasfresh/issues/12282) webui frontend: redux-* update 
  * [#12288](https://github.com/metasfresh/metasfresh/issues/12288) webui frontend: moment-timezone update
  * [#12289](https://github.com/metasfresh/metasfresh/issues/12289) webui frontend: reselect update
  * [#12294](https://github.com/metasfresh/metasfresh/issues/12294) webui frontend: storybook update 
  * [#12296](https://github.com/metasfresh/metasfresh/issues/12296) Modify C_BPartner: Add column OldValue, change column lengths
  * [#12298](https://github.com/metasfresh/metasfresh/issues/12298) Send additional Vendor Properties to GRS
  * [#12300](https://github.com/metasfresh/metasfresh/issues/12300) Receive additional Product Properties from GRS
  * [#12305](https://github.com/metasfresh/metasfresh/issues/12305) Fix translatation in all Windows "Advanced edit" to "Erweiterte Erfassung"
  * [#12307](https://github.com/metasfresh/metasfresh/issues/12307) Use org parameter when invoicing automatically
  * [#12312](https://github.com/metasfresh/metasfresh/issues/12312) shopware - Lookup contact of B2B customer
  * [#12314](https://github.com/metasfresh/metasfresh/issues/12314) Send extended bpartnerName to /orders/sales/candidates
  * [#12317](https://github.com/metasfresh/metasfresh/issues/12317) webui frontend: integrate menu icons pull request
  * [#12318](https://github.com/metasfresh/metasfresh/issues/12318) Add ability to explode BOM product in SO into its components when creating a PO for it
  * [#12323](https://github.com/metasfresh/metasfresh/issues/12323) Adding EORI Number to BPartner
  * [#12324](https://github.com/metasfresh/metasfresh/issues/12324) webui frontend: immer, autoprefixer, webpack, webpack-dev-server, @babel/register update to latest ver
  * [#12325](https://github.com/metasfresh/metasfresh/issues/12325) webui frontend: fix widget's right icon L&F 
  * [#12329](https://github.com/metasfresh/metasfresh/issues/12329) Export ShipmentCandidateAPIService needs switch between "Shopware" and "Oxid"
  * [#12334](https://github.com/metasfresh/metasfresh/issues/12334) Make sure csv exports open with UTF-8
  * [#12337](https://github.com/metasfresh/metasfresh/issues/12337) webui frontend: Fix number rounding
  * [#12344](https://github.com/metasfresh/metasfresh/issues/12344) Exchange HU-Data with GRS
  * [#12349](https://github.com/metasfresh/metasfresh/issues/12349) webui frontend: When loading a single document, if the network is slow, you will see for a while "There are no detail rows" in included tab
  * [#12351](https://github.com/metasfresh/metasfresh/issues/12351) webui frontend: Columns shifting on Components of the BOM & Formula
  * [#12356](https://github.com/metasfresh/metasfresh/issues/12356) Extend Attachment-API
  * [#12357](https://github.com/metasfresh/metasfresh/issues/12357) webui frontend: Harmonize loading gear on side list 
  * [#12359](https://github.com/metasfresh/metasfresh/issues/12359) webui frontend: Hide dashboard logo if we have items on dashboard
  * [#12360](https://github.com/metasfresh/metasfresh/issues/12360) Allow setting shipping costs by country area, not just by country.
  * [#12363](https://github.com/metasfresh/metasfresh/issues/12363) webui frontend: When searching in menu don't show There are no results while loading
  * [#12364](https://github.com/metasfresh/metasfresh/issues/12364) Exclude overdelivery after error by credit stop
  * [#12366](https://github.com/metasfresh/metasfresh/issues/12366) GRS Change ROLLE Array
  * [#12372](https://github.com/metasfresh/metasfresh/issues/12372) Support import formats linked to banks for bank statements
  * [#12383](https://github.com/metasfresh/metasfresh/issues/12383) webui frontend: Fix KPIs layout min/max size
  * [#12385](https://github.com/metasfresh/metasfresh/issues/12385) Replace `BIC` by `SwiftCode` in `Revolut_Payment_Export`
  * [#12387](https://github.com/metasfresh/metasfresh/issues/12387) Move the URL fields from `Product` tab to `Business Partner` tab in `Product` window
  * [#12394](https://github.com/metasfresh/metasfresh/issues/12394) GRS Changes around Vendor, Product an BOM
  * [#12397](https://github.com/metasfresh/metasfresh/issues/12397) Introduce IBAN Settings for different EU Countries 
  * [#12407](https://github.com/metasfresh/metasfresh/issues/12407) Add `SalesRep_ID` to BPartner and Sales Order window
  * [#12409](https://github.com/metasfresh/metasfresh/issues/12409) Copy shipto partner and address for SO order line to PO orderline
  * [#12414](https://github.com/metasfresh/metasfresh/issues/12414) Datev Export: Add type Provision Storno
  * [#12420](https://github.com/metasfresh/metasfresh/issues/12420) Add sysconfig that allows to set the offset for initial `PreparationDate` calculation
  * [#12422](https://github.com/metasfresh/metasfresh/issues/12422) externalsystems https EP shall provide better Error-infos
  * [#12435](https://github.com/metasfresh/metasfresh/issues/12435) General ledger journal debit/credit not updated
  * [#12442](https://github.com/metasfresh/metasfresh/issues/12442) GRS externalsystems creates folders on disk
  * [#12448](https://github.com/metasfresh/metasfresh/issues/12448) Make sure C_Order.Email ends up in C_DocOutbound_Log
  * [#12451](https://github.com/metasfresh/metasfresh/issues/12451) GRS - Also send Customers to GRS
  * [#12452](https://github.com/metasfresh/metasfresh/issues/12452) Alberta - order&product changes
  * [#12457](https://github.com/metasfresh/metasfresh/issues/12457) ExternalSystem_Other_ConfigParameter add description column
  * [#12468](https://github.com/metasfresh/metasfresh/issues/12468) Keyboard navigation in the attributes modal
  * [#12473](https://github.com/metasfresh/metasfresh/issues/12473) Create Product Certification window
  * [#12475](https://github.com/metasfresh/metasfresh/issues/12475) always set invoice-doctype when creating an IC for olc, ol and iol
  * [#12478](https://github.com/metasfresh/metasfresh/issues/12478) GRS sends locally stored attachments
  * [#12481](https://github.com/metasfresh/metasfresh/issues/12481) process MaterialEvents asynchronously
  * [#12483](https://github.com/metasfresh/metasfresh/issues/12483) Add Ireland IBAN Settings
  * [#12485](https://github.com/metasfresh/metasfresh/issues/12485) Purchaseand and sales Order incoterms filled from BP
  * [#12487](https://github.com/metasfresh/metasfresh/issues/12487) Add all related IBAN config fields to Web UI
  * [#12492](https://github.com/metasfresh/metasfresh/issues/12492) ASI Support in Product-BOM REST API
  * [#12493](https://github.com/metasfresh/metasfresh/issues/12493) Import Account: Set Parent From Import
  * [#12498](https://github.com/metasfresh/metasfresh/issues/12498) Fix tab sorting when using Lookups
  * [#12503](https://github.com/metasfresh/metasfresh/issues/12503) fix type for excel report : `Anbauplanung Auswertung Excel`
  * [#12511](https://github.com/metasfresh/metasfresh/issues/12511) remove `/v3` from Shopware calls
  * [#12518](https://github.com/metasfresh/metasfresh/issues/12518) Copy incoterm location from order to invoice and location
  * [#12520](https://github.com/metasfresh/metasfresh/issues/12520) material-dispo and unprocessed production-dispo need to update on new BOM version
  * [#12527](https://github.com/metasfresh/metasfresh/issues/12527) Implement HU-Locking
  * [#12529](https://github.com/metasfresh/metasfresh/issues/12529) shopware: receive customer => auto-send to rabbitmq
  * [#12534](https://github.com/metasfresh/metasfresh/issues/12534) Extend HUQRCode
  * [#12537](https://github.com/metasfresh/metasfresh/issues/12537) create BOM product price changes report
  * [#12539](https://github.com/metasfresh/metasfresh/issues/12539) GRS Change customer-JSON
  * [#12551](https://github.com/metasfresh/metasfresh/issues/12551) fix integration with DHL production environments
  * [#12552](https://github.com/metasfresh/metasfresh/issues/12552) shopware: renumber shopware-OLCand Lines
  * [#12566](https://github.com/metasfresh/metasfresh/issues/12566) Fix Jasper Report `C_Order_MFGWarehouse_Report_With_Barcode`
  * [#12570](https://github.com/metasfresh/metasfresh/issues/12570) Flexible Picking based on Age Attribute
  * [#12571](https://github.com/metasfresh/metasfresh/issues/12571) Shopware - Call using config's orgId instead of user role's orgId
  * [#12578](https://github.com/metasfresh/metasfresh/issues/12578) default PO warehouse
  * [#12580](https://github.com/metasfresh/metasfresh/issues/12580) In OLCandSetOverrideValues Infer location by GLN, for given bpartner
  * [#12583](https://github.com/metasfresh/metasfresh/issues/12583) Manufacturing candidate: filter by DateScheduled and Processed
  * [#12585](https://github.com/metasfresh/metasfresh/issues/12585) Display Tolerance Fileds in BOM Line and Manufacturing Order Line
  * [#12590](https://github.com/metasfresh/metasfresh/issues/12590) Products Proposal button should not be present under Order Tax Tab
  * [#12591](https://github.com/metasfresh/metasfresh/issues/12591) Overhaul QueueProcessor polling
  * [#12598](https://github.com/metasfresh/metasfresh/issues/12598) Call Order Contracts
  * [#12601](https://github.com/metasfresh/metasfresh/issues/12601) shopware - Automated testing for Siro and Invoicing
  * [#12608](https://github.com/metasfresh/metasfresh/issues/12608) Fix `Vendor` flag in `BPartnerQuickInputService`
  * [#12612](https://github.com/metasfresh/metasfresh/issues/12612) Fix logic for showing prices in Price list comparison report
  * [#12621](https://github.com/metasfresh/metasfresh/issues/12621) Mobilnummer im Kontakt der Organisation
  * [#12624](https://github.com/metasfresh/metasfresh/issues/12624) Quality discount in purchase invoice when QtyInvoiced < QtyReceived despite no quality issue in material receipt
  * [#12635](https://github.com/metasfresh/metasfresh/issues/12635) Set proper rendered address when creating Serial letters
  * [#12637](https://github.com/metasfresh/metasfresh/issues/12637) Allow product to have only prices with ASI
  * [#12640](https://github.com/metasfresh/metasfresh/issues/12640) M_MatchInv Window  Improvements
  * [#12641](https://github.com/metasfresh/metasfresh/issues/12641) Missing Translations (DE) Fix
  * [#12647](https://github.com/metasfresh/metasfresh/issues/12647) Do not allow modifying the product's uom if it already has uom conversions defined
  * [#12650](https://github.com/metasfresh/metasfresh/issues/12650) GRS add country attribute in BOM-component
  * [#12652](https://github.com/metasfresh/metasfresh/issues/12652) OLCand - Use internal packaging item capacity if feasible
  * [#12653](https://github.com/metasfresh/metasfresh/issues/12653) material dispo simulation
  * [#12660](https://github.com/metasfresh/metasfresh/issues/12660) Use Picking Terminal Config v2 in the Mobile UI picking
  * [#12662](https://github.com/metasfresh/metasfresh/issues/12662) HU-Clearance support for aggregated HUs
  * [#12663](https://github.com/metasfresh/metasfresh/issues/12663) Introduce M_InventoryLine.IsExplicitCostPrice flag
  * [#12669](https://github.com/metasfresh/metasfresh/issues/12669) Allow SEPA export `EndToEndId` param to be populated with payment reference (or NOTPROVIDED)
  * [#12670](https://github.com/metasfresh/metasfresh/issues/12670) Make Inventory with aggregated HUs doctype default
  * [#12673](https://github.com/metasfresh/metasfresh/issues/12673) Make SEPA export <BtchBookg> value configurable 
  * [#12675](https://github.com/metasfresh/metasfresh/issues/12675) GRS - Support multiple attachments in raw materials
  * [#12680](https://github.com/metasfresh/metasfresh/issues/12680) Call Order for the purchase side
  * [#12694](https://github.com/metasfresh/metasfresh/issues/12694) Pick via the "Received Amount"
  * [#12708](https://github.com/metasfresh/metasfresh/issues/12708) API Audit - fix weird error message in case of "non-routed" requests
  * [#12711](https://github.com/metasfresh/metasfresh/issues/12711) auto-sync external references metasfresh=>rabbitmq
  * [#12712](https://github.com/metasfresh/metasfresh/issues/12712) New Datev Export Format
  * [#12718](https://github.com/metasfresh/metasfresh/issues/12718) Fix inconsistent invoice BPLs
  * [#12721](https://github.com/metasfresh/metasfresh/issues/12721) Remove trailing whitespaces from INVOIC EDI exports EAN and GLN
  * [#12724](https://github.com/metasfresh/metasfresh/issues/12724) Display *** instead of text for columns containing the string "PW"
  * [#12728](https://github.com/metasfresh/metasfresh/issues/12728) Set ASI in receipt schedule
  * [#12737](https://github.com/metasfresh/metasfresh/issues/12737) Allow different number of copies for ordercheckup with barcode 
  * [#12739](https://github.com/metasfresh/metasfresh/issues/12739) API Audit - replay and cleanup improvements
  * [#12742](https://github.com/metasfresh/metasfresh/issues/12742) Extend pricelist excel export
  * [#12747](https://github.com/metasfresh/metasfresh/issues/12747) Fix replacement of bpartner locations
  * [#12751](https://github.com/metasfresh/metasfresh/issues/12751) Add `EMail` field in  SO  / Invoices / Invoice Candidates / Shipmets  Windows
  * [#12753](https://github.com/metasfresh/metasfresh/issues/12753) Add MHD geöffnet to product window 
  * [#12757](https://github.com/metasfresh/metasfresh/issues/12757) Increase M_Product_Trl Name from 60 to 80
  * [#12761](https://github.com/metasfresh/metasfresh/issues/12761) Differing Adresses lead to wrong bp-location display on metasfresh documents
  * [#12765](https://github.com/metasfresh/metasfresh/issues/12765) Mobile-UI and beyond: restrict un-cleared HUs
  * [#12770](https://github.com/metasfresh/metasfresh/issues/12770) Add new Instanze-Rule Type "Prevent base rollout"
  * [#12772](https://github.com/metasfresh/metasfresh/issues/12772) Write a process that causes an OOME
  * [#12783](https://github.com/metasfresh/metasfresh/issues/12783) Rename billing address and shipping address
  * [#12785](https://github.com/metasfresh/metasfresh/issues/12785) Shopware6 - Prevent NPE when unsetting companyName & error when different addresses point to same metasfresh address
  * [#12800](https://github.com/metasfresh/metasfresh/issues/12800) Rename Account Element to Chart of Accounts
  * [#12815](https://github.com/metasfresh/metasfresh/issues/12815) Add IsCloseInvoiceCandidate parameter when canceling contracts.
  * [#12830](https://github.com/metasfresh/metasfresh/issues/12830) Set compensated group id to orderLines in an ordered fashion
  * [#11751](https://github.com/metasfresh/metasfresh/pull/11751) Update CONTRIBUTING.md 
  * [#11923](https://github.com/metasfresh/metasfresh/pull/11923) Abort workflow button with prompt 
  * [#11928](https://github.com/metasfresh/metasfresh/pull/11928) Change partner for invoiced terms 
  * [#11933](https://github.com/metasfresh/metasfresh/pull/11933) mobile UI manufacturing prototype (2) 
  * [#11935](https://github.com/metasfresh/metasfresh/pull/11935) fulltextsearch.query.limit 
  * [#11936](https://github.com/metasfresh/metasfresh/pull/11936) PickFromHUsSupplier: hotfix consider all HUs, not only top level ones 
  * [#11937](https://github.com/metasfresh/metasfresh/pull/11937) Allow filtering Elasticsearch index by user role's orgs 
  * [#11946](https://github.com/metasfresh/metasfresh/pull/11946) mobile UI: create manufacturing issue plan 
  * [#11949](https://github.com/metasfresh/metasfresh/pull/11949) picking/unpicking fix corner cases 
  * [#11957](https://github.com/metasfresh/metasfresh/pull/11957) Distributions workflow
  * [#11958](https://github.com/metasfresh/metasfresh/pull/11958) Sql fo onboarding issues 2
  * [#11964](https://github.com/metasfresh/metasfresh/pull/11964) implement support for picking HU alternatives (backend)
  * [#11973](https://github.com/metasfresh/metasfresh/pull/11973) mobile UI: don't close the shipment schedules when we complete the picking job
  * [#11978](https://github.com/metasfresh/metasfresh/pull/11978) mobile UI: Pick using TUs support
  * [#11979](https://github.com/metasfresh/metasfresh/pull/11979) mobile UI frontend: fix broken application screen
  * [#11980](https://github.com/metasfresh/metasfresh/pull/11980) 5613400_sys_m_picking_job_step_pickedhu_fixes.sql
  * [#11981](https://github.com/metasfresh/metasfresh/pull/11981) mobile ui: picking job windows
  * [#11982](https://github.com/metasfresh/metasfresh/pull/11982) mobile UI frontend: Pick HU Alternatives
  * [#11989](https://github.com/metasfresh/metasfresh/pull/11989) Fixing the Zoom out of producing
  * [#11990](https://github.com/metasfresh/metasfresh/pull/11990) ensure positive service fee amount also for credit memos
  * [#11998](https://github.com/metasfresh/metasfresh/pull/11998) update the invoices' isPaid flag when allocation is completed
  * [#11999](https://github.com/metasfresh/metasfresh/pull/11999) use the current attachment's uploadDate as API param for the next call
  * [#12002](https://github.com/metasfresh/metasfresh/pull/12002) mobile UI: manufacturing issue
  * [#12003](https://github.com/metasfresh/metasfresh/pull/12003) fix spring security config
  * [#12005](https://github.com/metasfresh/metasfresh/pull/12005) Parameterized Address Layout (Address 3 /Address 4) via SysConf
  * [#12010](https://github.com/metasfresh/metasfresh/pull/12010) Intensive care hotfix creditmemo paid
  * [#12012](https://github.com/metasfresh/metasfresh/pull/12012) mobile UI: manufacturing receipt endpoint
  * [#12014](https://github.com/metasfresh/metasfresh/pull/12014) mobile UI: manufacturing receipt endpoint (3)
  * [#12015](https://github.com/metasfresh/metasfresh/pull/12015) mobile UI fix unit test & QAs
  * [#12021](https://github.com/metasfresh/metasfresh/pull/12021) mobile UI: mfg issue: provide qtyRejectedReasons
  * [#12022](https://github.com/metasfresh/metasfresh/pull/12022) QA
  * [#12023](https://github.com/metasfresh/metasfresh/pull/12023) mobile UI mfg issue: make sure step was not already issued
  * [#12024](https://github.com/metasfresh/metasfresh/pull/12024) mobile UI mfg close, compute correct status, fixes
  * [#12025](https://github.com/metasfresh/metasfresh/pull/12025) Manufacturing receipts & changes to mfg issues
  * [#12026](https://github.com/metasfresh/metasfresh/pull/12026) mobile UI distribution fixes
  * [#12027](https://github.com/metasfresh/metasfresh/pull/12027) mobile UI: receive qty endpoint: provide the total qty received so far
  * [#12030](https://github.com/metasfresh/metasfresh/pull/12030) mobile UI: mfg: provide manufacturing headers
  * [#12031](https://github.com/metasfresh/metasfresh/pull/12031) fix failing tests
  * [#12033](https://github.com/metasfresh/metasfresh/pull/12033) mobile UI: create distribution job in trx
  * [#12041](https://github.com/metasfresh/metasfresh/pull/12041) mobile UI fixes
  * [#12044](https://github.com/metasfresh/metasfresh/pull/12044) fix migration script
  * [#12045](https://github.com/metasfresh/metasfresh/pull/12045) fix hardcoded lang
  * [#12047](https://github.com/metasfresh/metasfresh/pull/12047) mobile UI: Fix trls
  * [#12048](https://github.com/metasfresh/metasfresh/pull/12048) Add attributes to product window
  * [#12053](https://github.com/metasfresh/metasfresh/pull/12053) Button for HU not found
  * [#12057](https://github.com/metasfresh/metasfresh/pull/12057) mobile UI frontend: distribution fixes
  * [#12062](https://github.com/metasfresh/metasfresh/pull/12062) mobile UI - HU Disposal prototype
  * [#12074](https://github.com/metasfresh/metasfresh/pull/12074) #12069 add marketplace window and  food related industry fields  in product window
  * [#12075](https://github.com/metasfresh/metasfresh/pull/12075) #12073 add po reference to invoice identifier
  * [#12076](https://github.com/metasfresh/metasfresh/pull/12076) Adding a new Additives window
  * [#12081](https://github.com/metasfresh/metasfresh/pull/12081) # add poreference to invoice identifier
  * [#12083](https://github.com/metasfresh/metasfresh/pull/12083)  move gh12073 migration script to a proper branch
  * [#12088](https://github.com/metasfresh/metasfresh/pull/12088) M_Warehouse.Manufacturing_Warehouse_Group_ID / M_Warehouse_Group table
  * [#12093](https://github.com/metasfresh/metasfresh/pull/12093) Adding nutritional data in product window
  * [#12100](https://github.com/metasfresh/metasfresh/pull/12100) Create label via REST-API
  * [#12103](https://github.com/metasfresh/metasfresh/pull/12103) mobile UI app: Inventory Disposal
  * [#12104](https://github.com/metasfresh/metasfresh/pull/12104) webui Manufacturing Issue/Receipt: consider mfg WH group when fetching source HUs
  * [#12107](https://github.com/metasfresh/metasfresh/pull/12107) ColumnSQL automatically set IsLazyLoading
  * [#12118](https://github.com/metasfresh/metasfresh/pull/12118) Set IsDropship and IsUseHandover flags when creating an order
  * [#12119](https://github.com/metasfresh/metasfresh/pull/12119) #cover material dispo with cucumber tests
  * [#12120](https://github.com/metasfresh/metasfresh/pull/12120) Don't show negative quantities in the prompt
  * [#12121](https://github.com/metasfresh/metasfresh/pull/12121) invalidate/update huge amount of ICs
  * [#12151](https://github.com/metasfresh/metasfresh/pull/12151) prefer shipmentSchedules that have HUs dedicated to them...
  * [#12153](https://github.com/metasfresh/metasfresh/pull/12153) fix around shipment schedule creation and allocation
  * [#12163](https://github.com/metasfresh/metasfresh/pull/12163) When alocating Qty and picking HUs on the fly, prefer reservations
  * [#12176](https://github.com/metasfresh/metasfresh/pull/12176) # add a reltype that points to service projects from sales order window
  * [#12177](https://github.com/metasfresh/metasfresh/pull/12177) # run archive_c_queue_data via scheduler
  * [#12178](https://github.com/metasfresh/metasfresh/pull/12178) #Fix mark-as-source-HU from component HUs #1255
  * [#12183](https://github.com/metasfresh/metasfresh/pull/12183) Adding new column Long Text Description to M_Product
  * [#12186](https://github.com/metasfresh/metasfresh/pull/12186) fix commission flaky tests
  * [#12194](https://github.com/metasfresh/metasfresh/pull/12194) Don't apply the rule if the salesrep has no margin contract
  * [#12203](https://github.com/metasfresh/metasfresh/pull/12203) Gh12202 maintaine address name
  * [#12220](https://github.com/metasfresh/metasfresh/pull/12220) Avoid cluttering the log with WorkpackageSkipRequestExceptions
  * [#12226](https://github.com/metasfresh/metasfresh/pull/12226) Avoid NPE
  * [#12229](https://github.com/metasfresh/metasfresh/pull/12229) avoid cluttering the log
  * [#12235](https://github.com/metasfresh/metasfresh/pull/12235) Gh12210 add parameter spreadsheet format
  * [#12246](https://github.com/metasfresh/metasfresh/pull/12246) Add extra safety check for calling getData within handleChangePage
  * [#12249](https://github.com/metasfresh/metasfresh/pull/12249) Don't consider terms as overlapping that have different AD_Org_IDs
  * [#12257](https://github.com/metasfresh/metasfresh/pull/12257) get_C_ValidCombination_Records: QA & improvements
  * [#12261](https://github.com/metasfresh/metasfresh/pull/12261) assert_period_open_by_record: handle C_Payment
  * [#12262](https://github.com/metasfresh/metasfresh/pull/12262) 12254 e2e begin jan2022
  * [#12267](https://github.com/metasfresh/metasfresh/pull/12267) Improve retrieval performance of workpackage items for WP processors
  * [#12268](https://github.com/metasfresh/metasfresh/pull/12268) Add new exportdate and exportby colums in table DatevAcctExport
  * [#12270](https://github.com/metasfresh/metasfresh/pull/12270) DatevExportType (AD_Reference) Reference corrections
  * [#12275](https://github.com/metasfresh/metasfresh/pull/12275) 12263 update prettier eslint
  * [#12280](https://github.com/metasfresh/metasfresh/pull/12280) On view changed WS event, avoid unnecessary refreshes
  * [#12287](https://github.com/metasfresh/metasfresh/pull/12287) gh12234_Include_features_in_inventory_position_counting
  * [#12291](https://github.com/metasfresh/metasfresh/pull/12291) Update version.properties
  * [#12292](https://github.com/metasfresh/metasfresh/pull/12292) Additive Trl corrections
  * [#12297](https://github.com/metasfresh/metasfresh/pull/12297) #correct trls for alternative products
  * [#12304](https://github.com/metasfresh/metasfresh/pull/12304) Kickstart HU Manager application
  * [#12306](https://github.com/metasfresh/metasfresh/pull/12306) Gh12305
  * [#12319](https://github.com/metasfresh/metasfresh/pull/12319) Fix compile errors (java 15); QA
  * [#12339](https://github.com/metasfresh/metasfresh/pull/12339) HU QR Codes [ WIP ]
  * [#12341](https://github.com/metasfresh/metasfresh/pull/12341) Adding EORI Number and it shall be printed on each document
  * [#12343](https://github.com/metasfresh/metasfresh/pull/12343) translate Advanced Edit popup
  * [#12345](https://github.com/metasfresh/metasfresh/pull/12345) set the Export Date only when using this process (In Datei speichern)
  * [#12355](https://github.com/metasfresh/metasfresh/pull/12355) Drop foreign-key-constraints for AD_Issue_ID and AD_PInstance_ID
  * [#12374](https://github.com/metasfresh/metasfresh/pull/12374) Log migration scripts context info
  * [#12375](https://github.com/metasfresh/metasfresh/pull/12375) GRS-Mappings documentation
  * [#12377](https://github.com/metasfresh/metasfresh/pull/12377) fix flaky checkInvoiceCandStatusand invoiceRules cucumber
  * [#12390](https://github.com/metasfresh/metasfresh/pull/12390) Bump commons-io from 2.5 to 2.7 in /misc/de-metas-common/de-metas-common-externalsystem
  * [#12391](https://github.com/metasfresh/metasfresh/pull/12391) Replace BIC by SwiftCode in Revolut Export
  * [#12400](https://github.com/metasfresh/metasfresh/pull/12400) Move the URL fields from Product tab to Business Partner tab in Produ…
  * [#12406](https://github.com/metasfresh/metasfresh/pull/12406) Auto height for dashboard kpi
  * [#12412](https://github.com/metasfresh/metasfresh/pull/12412) fix CZ accountnumberlength; add additional tests
  * [#12418](https://github.com/metasfresh/metasfresh/pull/12418) [ HOTFIX ] When printing C_Letter, consider the configurated Jasper from boilerplate if any
  * [#12428](https://github.com/metasfresh/metasfresh/pull/12428) Gh12420 add preparation date offset
  * [#12441](https://github.com/metasfresh/metasfresh/pull/12441) Add Offset as Hours
  * [#12443](https://github.com/metasfresh/metasfresh/pull/12443) Fix attributes request
  * [#12444](https://github.com/metasfresh/metasfresh/pull/12444) gh12424: adjust Trls for PO window
  * [#12447](https://github.com/metasfresh/metasfresh/pull/12447) DefaultView.afterDestroy: cleanup webui selections [ PROTOTYPE ]
  * [#12456](https://github.com/metasfresh/metasfresh/pull/12456) #gh1345 : Make sure that M_Replenish LevelMax is >= LevelMin
  * [#12461](https://github.com/metasfresh/metasfresh/pull/12461) update README file
  * [#12462](https://github.com/metasfresh/metasfresh/pull/12462) PickingCandidateRepository: load only the picking candidates for our already fetched picking slots
  * [#12463](https://github.com/metasfresh/metasfresh/pull/12463) PickingCandidateRepository: don't load HU attributes because they are not needed anyways
  * [#12464](https://github.com/metasfresh/metasfresh/pull/12464) Fix tests after tasty_ham_merge
  * [#12466](https://github.com/metasfresh/metasfresh/pull/12466) order's effective bill-contact - only fall back if consistent
  * [#12470](https://github.com/metasfresh/metasfresh/pull/12470) HOTFIX: Accept: application/json when connecting to remote json REST API
  * [#12472](https://github.com/metasfresh/metasfresh/pull/12472) IdsToFilter.streamSingleValues shall return empty if no value
  * [#12480](https://github.com/metasfresh/metasfresh/pull/12480) Purchaseand and sales Order incoterms filled from BP
  * [#12489](https://github.com/metasfresh/metasfresh/pull/12489) HU QR Code (part 2)
  * [#12491](https://github.com/metasfresh/metasfresh/pull/12491) gh12490:Activate RelType with isTableRecordIDTarget = Y
  * [#12510](https://github.com/metasfresh/metasfresh/pull/12510) Add a process to select a HU in HU editor, scan a QR Code and assign that QR code to that HU
  * [#12514](https://github.com/metasfresh/metasfresh/pull/12514) hotfix text input does not react to pasted text
  * [#12515](https://github.com/metasfresh/metasfresh/pull/12515) fix mobile UI trls
  * [#12521](https://github.com/metasfresh/metasfresh/pull/12521) change TU-uoms to PCE when sending DESADVs
  * [#12522](https://github.com/metasfresh/metasfresh/pull/12522)  use the dropship location as store number and name
  * [#12528](https://github.com/metasfresh/metasfresh/pull/12528) mobile UI scale devices support
  * [#12530](https://github.com/metasfresh/metasfresh/pull/12530) Use org from element value
  * [#12533](https://github.com/metasfresh/metasfresh/pull/12533) bump edi to java-17
  * [#12545](https://github.com/metasfresh/metasfresh/pull/12545) Locator QR Code support
  * [#12546](https://github.com/metasfresh/metasfresh/pull/12546) Picking Slot QR Code
  * [#12547](https://github.com/metasfresh/metasfresh/pull/12547) mobile UI: Move HU
  * [#12555](https://github.com/metasfresh/metasfresh/pull/12555) hotfix exception on destroying an empty aggregated TU
  * [#12557](https://github.com/metasfresh/metasfresh/pull/12557) #gh12550: Order entry default delivery address and contact is not set
  * [#12558](https://github.com/metasfresh/metasfresh/pull/12558) hotfix: Split out one active TU from a LU with aggregated TUs
  * [#12559](https://github.com/metasfresh/metasfresh/pull/12559) mobile UI: move HU - before moving, split out HU, if needed
  * [#12563](https://github.com/metasfresh/metasfresh/pull/12563) HUQRCode support when filtering by barcodes in webui views
  * [#12564](https://github.com/metasfresh/metasfresh/pull/12564) Manufacturing Issue Tolerance | Issue Adjustment Step [ PROTOTYPE ]
  * [#12565](https://github.com/metasfresh/metasfresh/pull/12565) Setting clearance in mobileui
  * [#12569](https://github.com/metasfresh/metasfresh/pull/12569) Don't check ASI mandatory on movement. This prevents us from moving HUs.
  * [#12573](https://github.com/metasfresh/metasfresh/pull/12573) mobile UI: HU Manager: Show if disposing
  * [#12574](https://github.com/metasfresh/metasfresh/pull/12574) mobile UI: fix mfg generate HU QR codes
  * [#12575](https://github.com/metasfresh/metasfresh/pull/12575) mobile UI: distribution fixes (after global QR codes)
  * [#12576](https://github.com/metasfresh/metasfresh/pull/12576) mobile UI: distribution: DD Order shall work on top level HUs only (for now)
  * [#12577](https://github.com/metasfresh/metasfresh/pull/12577) mobile UI: HU Manager: show HU attributes
  * [#12586](https://github.com/metasfresh/metasfresh/pull/12586) de.metas.order.model.interceptor.C_Order#setIncoterms should also be …
  * [#12593](https://github.com/metasfresh/metasfresh/pull/12593) Fixes for dropship delivery and material tracking
  * [#12594](https://github.com/metasfresh/metasfresh/pull/12594) mobile UI: HU Manager: avoid not physical HUs
  * [#12595](https://github.com/metasfresh/metasfresh/pull/12595) mobile UI: abort Picking Job on sales order close
  * [#12599](https://github.com/metasfresh/metasfresh/pull/12599) Save vendor attribute
  * [#12600](https://github.com/metasfresh/metasfresh/pull/12600) metasfresh - procurement audit
  * [#12609](https://github.com/metasfresh/metasfresh/pull/12609) #gh12607: cant copy product window
  * [#12622](https://github.com/metasfresh/metasfresh/pull/12622) #gh12621: add user communication info in user window
  * [#12623](https://github.com/metasfresh/metasfresh/pull/12623) Accounting support functions improvements & fixes
  * [#12626](https://github.com/metasfresh/metasfresh/pull/12626) augment the message send to metasfresh when a shopware order is skipped
  * [#12628](https://github.com/metasfresh/metasfresh/pull/12628) Hard encoded esr trx inherited
  * [#12630](https://github.com/metasfresh/metasfresh/pull/12630) call order cucumber
  * [#12644](https://github.com/metasfresh/metasfresh/pull/12644) further testing for Siro and Invoicing
  * [#12646](https://github.com/metasfresh/metasfresh/pull/12646) step def data refactoring
  * [#12649](https://github.com/metasfresh/metasfresh/pull/12649) Updated translations for "Import Format - Subscritions"
  * [#12655](https://github.com/metasfresh/metasfresh/pull/12655) webui: fix sorting by multiple columns
  * [#12659](https://github.com/metasfresh/metasfresh/pull/12659) webui Payment Allocations: don't close the invoices included view when unselecting the payment row
  * [#12667](https://github.com/metasfresh/metasfresh/pull/12667) webui frontend: Date/Time widget fixes
  * [#12689](https://github.com/metasfresh/metasfresh/pull/12689) MarginCommission: get product sales rep product price by SHIP_TO
  * [#12690](https://github.com/metasfresh/metasfresh/pull/12690) Add Test.M_AttributeSetInstance_ID column
  * [#12702](https://github.com/metasfresh/metasfresh/pull/12702) QA/cleanup AD_Schedule manage code
  * [#12703](https://github.com/metasfresh/metasfresh/pull/12703) Window Reference - Tab Used in Process Params
  * [#12714](https://github.com/metasfresh/metasfresh/pull/12714) On view changed WS event, remove missing rows  

## Fixes
* metasfresh
  * [#14117](https://github.com/metasfresh/metasfresh/issues/14117) fix after migration failure
  * [#13174](https://github.com/metasfresh/metasfresh/pull/13174) wrap DateAcct with TRUNC while looking for a C_Period
  * [#13100](https://github.com/metasfresh/metasfresh/issues/13100) Overhaul Shipments interaction with Material Schedule 
  * [#11931](https://github.com/metasfresh/metasfresh/issues/11931) Address is not saved when focus is on other tab
  * [#12017](https://github.com/metasfresh/metasfresh/issues/12017) UnpackV2ResponseRouteBuilder should not fail for "not-wrapped" api responses
  * [#12105](https://github.com/metasfresh/metasfresh/issues/12105) Picking error: huId is null
  * [#12208](https://github.com/metasfresh/metasfresh/issues/12208) BUG: ship with picked on the fly HU
  * [#12273](https://github.com/metasfresh/metasfresh/pull/12273) Activity Fix
  * [#12276](https://github.com/metasfresh/metasfresh/issues/12276) Solve duplicate key value violates unique constraint "c_bpartner_product_stats_uq" error
  * [#12393](https://github.com/metasfresh/metasfresh/issues/12393) Fix InvoiceProcessingServiceCompanyService#isServiceInvoiceAlreadyGenerated
  * [#12561](https://github.com/metasfresh/metasfresh/issues/12561) Produktübertrag nach alberta Problem
  * [#12606](https://github.com/metasfresh/metasfresh/pull/12606) C_OLCand.QtyShipped: distinguish between <=0 and "unspecified" 


# metasfresh 5.174
## Features
* metasfresh
  * [#13234](https://github.com/metasfresh/metasfresh/issues/13234) Clicking outside a dropdown field w/o selection does not close the dropdown                                                                                                 
  * [#11508](https://github.com/metasfresh/metasfresh/issues/11508) Implement ESR payment action - duplicate payment
  * [#11679](https://github.com/metasfresh/metasfresh/issues/11679) New Cancel and recreate ("Stornieren und neu erstellen") process
  * [#11701](https://github.com/metasfresh/metasfresh/issues/11701) Add organization-based filter for currently logged-in user: `OrgAccessSql`
  * [#11720](https://github.com/metasfresh/metasfresh/issues/11720) Margin Commission
  * [#11728](https://github.com/metasfresh/metasfresh/issues/11728) Allow contract discounts based on time of subscription creation
  * [#11737](https://github.com/metasfresh/metasfresh/pull/11737) Workflow & Picking REST API prototype [master branch]
  * [#11744](https://github.com/metasfresh/metasfresh/issues/11744) Create Unique indexes for Fachrichtung tables
  * [#11748](https://github.com/metasfresh/metasfresh/issues/11748) Add a FK on `ESR_Import.AD_Attachmententry_ID`
  * [#11750](https://github.com/metasfresh/metasfresh/issues/11750) Support also n:1 connections between sales and purchase order lines
  * [#11758](https://github.com/metasfresh/metasfresh/issues/11758) Implement possibility to set sales order line in manufacturing order
  * [#11762](https://github.com/metasfresh/metasfresh/issues/11762) Extend v2-BPartner-JSON
  * [#11763](https://github.com/metasfresh/metasfresh/issues/11763) ESR Import: cut "/" and anything after in Post-Teilnehmernummer
  * [#11767](https://github.com/metasfresh/metasfresh/pull/11767) Fix and update Swagger-UI
  * [#11769](https://github.com/metasfresh/metasfresh/issues/11769) Cucumber improvements
  * [#11771](https://github.com/metasfresh/metasfresh/pull/11771) Sort attachment entries by created timestamp - youngest first
  * [#11772](https://github.com/metasfresh/metasfresh/issues/11772) Process to close all terms for a `Flatrate_Data` entry
  * [#11774](https://github.com/metasfresh/metasfresh/pull/11774) Blonde monkey hotfix internal name length
  * [#11776](https://github.com/metasfresh/metasfresh/pull/11776) Delete `X_MRP_ProductInfo_Detail_MV` and `X_MRP_ProductInfo_V`
  * [#11777](https://github.com/metasfresh/metasfresh/pull/11777) Add DB function to reindex bpartners into elastic search
  * [#11784](https://github.com/metasfresh/metasfresh/issues/11784) Extend behavior for OLCand with sales-reps
  * [#11789](https://github.com/metasfresh/metasfresh/issues/11789) Table Org Permissions
  * [#11797](https://github.com/metasfresh/metasfresh/issues/11797) Specify designated vendor in sales order line
  * [#11798](https://github.com/metasfresh/metasfresh/issues/11798) Import products from Shopware
  * [#11803](https://github.com/metasfresh/metasfresh/issues/11803) Create Incoterms Tables and window
  * [#11806](https://github.com/metasfresh/metasfresh/issues/11806) Use the safe UOM-Price-Conversion method
  * [#11812](https://github.com/metasfresh/metasfresh/issues/11812) Implemented vendor attribute
  * [#11814](https://github.com/metasfresh/metasfresh/issues/11814) Material Cockpit changes
  * [#11817](https://github.com/metasfresh/metasfresh/issues/11817) Add `C_order.C_BPartner_Pharmacy_ID` column
  * [#11818](https://github.com/metasfresh/metasfresh/issues/11818) Create new Tab "Contract period curr. year" in window Vertragspartner
  * [#11821](https://github.com/metasfresh/metasfresh/issues/11821) Create an external system config "GRS SIGNUM"
  * [#11822](https://github.com/metasfresh/metasfresh/issues/11822) Create missing Relation Types
  * [#11829](https://github.com/metasfresh/metasfresh/pull/11829) [ MAJOR ] Change the way we build FilterSql results
  * [#11831](https://github.com/metasfresh/metasfresh/issues/11831) Display Brutto Weight Zollrechnung
  * [#11832](https://github.com/metasfresh/metasfresh/issues/11832) Auto-add attachments to mail
  * [#11834](https://github.com/metasfresh/metasfresh/issues/11834) Overhaul and propagate fields from Alberta to order
  * [#11836](https://github.com/metasfresh/metasfresh/pull/11836) Quick Input - more features
  * [#11840](https://github.com/metasfresh/metasfresh/issues/11840) System admin role always `iswebuirole` = `Y`
  * [#11841](https://github.com/metasfresh/metasfresh/issues/11841) API - Allow Shopware6 to invoke external system with `OrderId`
  * [#11843](https://github.com/metasfresh/metasfresh/issues/11843) Additional fields in Business Partner quick input contact
  * [#11847](https://github.com/metasfresh/metasfresh/issues/11847) Implementing a process that shall update product and all related data in a contract
  * [#11848](https://github.com/metasfresh/metasfresh/issues/11848) Receive vendor master data from GRS
  * [#11850](https://github.com/metasfresh/metasfresh/issues/11850) Allow address changes to be entered with a future date
  * [#11851](https://github.com/metasfresh/metasfresh/issues/11851) Request and notification for partner created from another org
  * [#11854](https://github.com/metasfresh/metasfresh/issues/11854) Process to change Flatrate Term's partner, location and user
  * [#11860](https://github.com/metasfresh/metasfresh/issues/11860) Receive Product master data from GRS
  * [#11863](https://github.com/metasfresh/metasfresh/issues/11863) Extend externalsystems-camel to write an audit trail
  * [#11864](https://github.com/metasfresh/metasfresh/issues/11864) Set the sales rep from order to inout
  * [#11866](https://github.com/metasfresh/metasfresh/issues/11866) New Invoice Rule: after Pick
  * [#11872](https://github.com/metasfresh/metasfresh/issues/11872) Set invoice doc types to invoice candidates in the flatrate term handler
  * [#11873](https://github.com/metasfresh/metasfresh/issues/11873) Set location value to invoice candidates in the flatrate term handler
  * [#11880](https://github.com/metasfresh/metasfresh/issues/11880) Import shopware product prices
  * [#11884](https://github.com/metasfresh/metasfresh/issues/11884) Allow setting a P.O. Box as business partner address
  * [#11890](https://github.com/metasfresh/metasfresh/issues/11890) Automatic Shipping and Invoicing
  * [#11898](https://github.com/metasfresh/metasfresh/issues/11898) Create `C_SubscriptionProgress` records on quantity and price changes
  * [#11906](https://github.com/metasfresh/metasfresh/issues/11906) Additional Products for migrated contracts
  * [#11908](https://github.com/metasfresh/metasfresh/issues/11908) Support `#AD_Org_ID` in `AD_Tab.WhereClause`
  * [#11909](https://github.com/metasfresh/metasfresh/issues/11909) Delete obsolete public class `IReferenceNoGenerators`
  * [#11912](https://github.com/metasfresh/metasfresh/pull/11912) Hash version injection
  * [#11918](https://github.com/metasfresh/metasfresh/pull/11918) Mobile UI manufacturing prototype (first iteration)
  * [#11922](https://github.com/metasfresh/metasfresh/pull/11922) Mobile UI: pick from alternatives prototype

## Fixes
* metasfresh
  * [#11766](https://github.com/metasfresh/metasfresh/issues/11766) Fix missing `M_HU_BestBefore_V_ID` column in `M_HU_BestBefore_V`
  * [#11778](https://github.com/metasfresh/metasfresh/issues/11778) Change Delivery Via Rule when Business Partner is changed
  * [#11780](https://github.com/metasfresh/metasfresh/issues/11780) Bugfix: create sales order form proposal
  * [#11786](https://github.com/metasfresh/metasfresh/pull/11786) Invalidate bpartner-API-cache if `C_User_Assigned_Role` was changed
  * [#11791](https://github.com/metasfresh/metasfresh/issues/11791) Fix `S_ExternalProjectReference` UC
  * [#11792](https://github.com/metasfresh/metasfresh/pull/11792) `JSONDocumentReferencesEventPublisher`: explicitly send JSON
  * [#11793](https://github.com/metasfresh/metasfresh/issues/11793) Delete User Dependency before deleting the User
  * [#11800](https://github.com/metasfresh/metasfresh/issues/11800) Invalidate API-cache when user-role-label is changed
  * [#11802](https://github.com/metasfresh/metasfresh/pull/11802) Fix error when building with npm
  * [#11809](https://github.com/metasfresh/metasfresh/issues/11809) Window content doesn't change when opening another window
  * [#11810](https://github.com/metasfresh/metasfresh/issues/11810) Fix Distributionsauftrag document sequence, TRL and actions
  * [#11823](https://github.com/metasfresh/metasfresh/pull/11823) Fix known commission-bugs
  * [#11825](https://github.com/metasfresh/metasfresh/issues/11825) Error when trying to set subproducer in HU Editor
  * [#11838](https://github.com/metasfresh/metasfresh/issues/11838) Make sure that the org is sent to `report_footer` in all reports
  * [#11856](https://github.com/metasfresh/metasfresh/issues/11856) Add Missing TRL Marketing Platform
  * [#11858](https://github.com/metasfresh/metasfresh/pull/11858) External system - Fix path mapping
  * [#11868](https://github.com/metasfresh/metasfresh/issues/11868) Checkboxes in tab's table not saved correctly
  * [#11895](https://github.com/metasfresh/metasfresh/issues/11895) Partner Location dropdown not taking full width
  * [#11897](https://github.com/metasfresh/metasfresh/pull/11897) Material schedule fixes
  * [#11913](https://github.com/metasfresh/metasfresh/issues/11913) WebUI frontend: Password component: show password button does nothing

# metasfresh 5.173
## Features
* metasfresh
  * [#11607](https://github.com/metasfresh/metasfresh/issues/11607) FE package updates - chunk 3 mid August
  * [#11624](https://github.com/metasfresh/metasfresh/issues/11624) FE: option to always display "New BPartner" in order
  * [#11654](https://github.com/metasfresh/metasfresh/issues/11654) Create Occupation Hierarchy tables and Validation Rules
  * [#11665](https://github.com/metasfresh/metasfresh/issues/11665) C&E User / BPartner Synchronisation metasfresh => RabbitMQ
  * [#11668](https://github.com/metasfresh/metasfresh/issues/11668) Chunk e2e for end of August 2021
  * [#11694](https://github.com/metasfresh/metasfresh/issues/11694) Commission Calculation for Purchase Order Forwarding
  * [#11698](https://github.com/metasfresh/metasfresh/issues/11698) Check and see more of the react* deps that can be updated and adapt code with the changes
  * [#11699](https://github.com/metasfresh/metasfresh/issues/11699) Chunk e2e beginning of Sep 2021
  * [#11701](https://github.com/metasfresh/metasfresh/issues/11701) Add organization-based filter for currently logged-in user: `OrgAccessSql`
  * [#11713](https://github.com/metasfresh/metasfresh/issues/11713) Add `DeliveryViaRule` to DESADV
  * [#11734](https://github.com/metasfresh/metasfresh/issues/11734) Add `isActive` Filter to window Product Price

## Fixes
* metasfresh
  * [#11680](https://github.com/metasfresh/metasfresh/pull/11680) Fix `ESRDataImporterCamt54` context switching issues

# metasfresh 5.172
## Features
* metasfresh
  * [#11006](https://github.com/metasfresh/metasfresh/pull/11006) Persist and forward the current `C_Location_ID`
  * [#11476](https://github.com/metasfresh/metasfresh/pull/11476) New Cost Estimate doctype and report
  * [#11525](https://github.com/metasfresh/metasfresh/issues/11525) ESR Import with zip files
  * [#11547](https://github.com/metasfresh/metasfresh/issues/11547) Smoothen the experience of connecting to shopware
  * [#11578](https://github.com/metasfresh/metasfresh/pull/11578) BPartner full text search
  * [#11587](https://github.com/metasfresh/metasfresh/issues/11587) Implement possibility to hide order lines
  * [#11600](https://github.com/metasfresh/metasfresh/issues/11600) Budget für Mitarbeiter 2
  * [#11605](https://github.com/metasfresh/metasfresh/issues/11605) Add ability to prevent sale of items under a certain qty
  * [#11611](https://github.com/metasfresh/metasfresh/issues/11611) Ability to use variables when sending email via `MailWorkpackageProcessor`
  * [#11616](https://github.com/metasfresh/metasfresh/pull/11616) Business partner window: field statuses
  * [#11617](https://github.com/metasfresh/metasfresh/issues/11617) Option to always display "New BPartner" in order
  * [#11620](https://github.com/metasfresh/metasfresh/pull/11620) Show no choice available in case mandatory is true and there are no results in the list
  * [#11625](https://github.com/metasfresh/metasfresh/issues/11625) Add in the messages API endpoint `No results found` strings
  * [#11630](https://github.com/metasfresh/metasfresh/issues/11630) Modal overlay for purchase order attachments
  * [#11631](https://github.com/metasfresh/metasfresh/issues/11631) BPartner location name should be made unique, and consistent with
  * [#11636](https://github.com/metasfresh/metasfresh/issues/11636) Modification to window Ingredients and Change Product Specification Report
  * [#11640](https://github.com/metasfresh/metasfresh/issues/11640) Automated order, shipment & invoice generation
  * [#11643](https://github.com/metasfresh/metasfresh/issues/11643) Create a membership month structure
  * [#11647](https://github.com/metasfresh/metasfresh/issues/11647) Extend Boiler plates to product category and document type
  * [#11651](https://github.com/metasfresh/metasfresh/issues/11651) FE package updates - chunk 4 end of August 2021
  * [#11657](https://github.com/metasfresh/metasfresh/issues/11657) Add new boiler plate structure to sales order jasper report
  * [#11662](https://github.com/metasfresh/metasfresh/issues/11662) Roles for `AD_User`, with possibility of restricting to one user for a role per business partner
  * [#11670](https://github.com/metasfresh/metasfresh/issues/11670) Disable the tutorial feature temporary and the loaded deps
  * [#11681](https://github.com/metasfresh/metasfresh/pull/11681) Full text search improvements
  * [#11685](https://github.com/metasfresh/metasfresh/issues/11685) WebUI frontend: show a loading/spinner while the search assistant modal is loading

## Fixes
* metasfresh
  * [#11573](https://github.com/metasfresh/metasfresh/issues/11573) Prevent bpartner logic selecting a shipping-location without `isShipTo='Y'`
  * [#11588](https://github.com/metasfresh/metasfresh/issues/11588) Prevent same HU being returned multiple times
  * [#11615](https://github.com/metasfresh/metasfresh/issues/11615) FE - Fields in bpartner issue should reflect their own status, not the bpartner field's status
  * [#11622](https://github.com/metasfresh/metasfresh/issues/11622) Replace the empty hardcoded strings passed to `SelectionDropdown` component
  * [#11627](https://github.com/metasfresh/metasfresh/issues/11627) The context menu jumps when opening in sub tab records
  * [#11638](https://github.com/metasfresh/metasfresh/pull/11638) Avoid NPE if referenced `C_SubscriptionProgress` is gone
  * [#11649](https://github.com/metasfresh/metasfresh/pull/11649) Master transportation order bug
  * [#11656](https://github.com/metasfresh/metasfresh/pull/11656) Fix shopware-camel problems
  * [#11659](https://github.com/metasfresh/metasfresh/pull/11659) Shopware - Fix problem with missing freight-costs if tax=0
  * [#11661](https://github.com/metasfresh/metasfresh/pull/11661) Increase the web-api-client's buffer-size to 50MB
  * [#11667](https://github.com/metasfresh/metasfresh/issues/11667) Fix function `report.taxnote(p_c_invoice_id numeric);`
  * [#11674](https://github.com/metasfresh/metasfresh/issues/11674) Align Problem on Label Fields
  * [#11675](https://github.com/metasfresh/metasfresh/issues/11675) Problem on Label Fields selection
  * [#11684](https://github.com/metasfresh/metasfresh/pull/11684) BP Quick Input: assert price lists exist

# metasfresh 5.171
## Features
* metasfresh
  * [#11015](https://github.com/metasfresh/metasfresh/issues/11015) Move frontend to react-router v5
  * [#11369](https://github.com/metasfresh/metasfresh/issues/11369) Display Label fileds in Grid view
  * [#11436](https://github.com/metasfresh/metasfresh/issues/11436) Supplier Approval Strategy
  * [#11437](https://github.com/metasfresh/metasfresh/pull/11437) material-dispo supports stock-estimate events
  * [#11447](https://github.com/metasfresh/metasfresh/issues/11447) Adding TRLs for Service Annahme and Request window and Change PO Reference in `m_inout` table to be identifier
  * [#11457](https://github.com/metasfresh/metasfresh/issues/11457) Automatic creditorId/DebitorId update when `c_bpartner.value` changes
  * [#11458](https://github.com/metasfresh/metasfresh/issues/11458) Create `C_BP_Relation.IsBranchOffice` and display it in Partner Relation window
  * [#11470](https://github.com/metasfresh/metasfresh/issues/11470) `PP_Order_RecordWork` should support decimal duration values
  * [#11473](https://github.com/metasfresh/metasfresh/issues/11473) Implement the possibility to allow auto allocation with next invoice when importing ESR
  * [#11478](https://github.com/metasfresh/metasfresh/issues/11478) REMADV related tweaks
  * [#11484](https://github.com/metasfresh/metasfresh/issues/11484) Create Validation Rule for `C_BPartner_Patient_ID`, `C_BPartner_Doctor_ID` and `C_BPartner_Pharmacy_ID`. New `C_Order_ID` and `C_BPartner_Payer_ID` in `Alberta_PrescriptionRequest` Table
  * [#11488](https://github.com/metasfresh/metasfresh/issues/11488) Create `C_CommissionShare` for sales partners without commission contract
  * [#11489](https://github.com/metasfresh/metasfresh/issues/11489) Add Offer No in sales order description function
  * [#11501](https://github.com/metasfresh/metasfresh/issues/11501) `AD_Process`: Export to CSV
  * [#11507](https://github.com/metasfresh/metasfresh/issues/11507) Remove all unnecessary and erroneous messages from unit tests log
  * [#11508](https://github.com/metasfresh/metasfresh/issues/11508) Implement ESR payment action - duplicate payment
  * [#11514](https://github.com/metasfresh/metasfresh/pull/11514) Remove `HUDescriptor#quantityDelta`, it wasn't used and created confusion
  * [#11516](https://github.com/metasfresh/metasfresh/issues/11516) Time-booking window - indicate if parent is already invoiced there as well
  * [#11522](https://github.com/metasfresh/metasfresh/issues/11522) New Values for Alberta Therapy and Alberta Therapy Type
  * [#11527](https://github.com/metasfresh/metasfresh/pull/11527) Avoid OOME by using spring Resource instead of byte[]
  * [#11529](https://github.com/metasfresh/metasfresh/issues/11529) Tell camel from metasfresh to open http-EP with particular auth-token
  * [#11534](https://github.com/metasfresh/metasfresh/pull/11534) Order lookup results by levenshtein distance
  * [#11535](https://github.com/metasfresh/metasfresh/issues/11535) DB-Function for customizable DB-changes on DB-transfer
  * [#11539](https://github.com/metasfresh/metasfresh/issues/11539) PaySelection CSV-File export for Revolut
  * [#11543](https://github.com/metasfresh/metasfresh/issues/11543) Remove legacy MRP info window code
  * [#11545](https://github.com/metasfresh/metasfresh/pull/11545) Display labels in grid mode
  * [#11551](https://github.com/metasfresh/metasfresh/issues/11551) WebUI Display `AD_Element` Description also in class based views
  * [#11554](https://github.com/metasfresh/metasfresh/issues/11554) Update react-tether package
  * [#11571](https://github.com/metasfresh/metasfresh/issues/11571) Packages update August 2021
  * [#11575](https://github.com/metasfresh/metasfresh/issues/11575) Remove all uses of immutable.js
  * [#11580](https://github.com/metasfresh/metasfresh/issues/11580) Update relevant tabs when workflow field is updated on manufacturing order
  * [#11590](https://github.com/metasfresh/metasfresh/issues/11590) Allow order discount via API (compensation group)
  * [#11595](https://github.com/metasfresh/metasfresh/issues/11595) FE package updates - chunk mid August
  * [#11597](https://github.com/metasfresh/metasfresh/issues/11597) Gebindesaldo - Improve M_Material_Balance_Config Standard Name

## Fixes
* metasfresh
  * [#10900](https://github.com/metasfresh/metasfresh/issues/10900) WebUI frontend: Fix breadcrumb issues for good
  * [#11415](https://github.com/metasfresh/metasfresh/issues/11415) Fix menue tree on releasetestit and instancesuat
  * [#11474](https://github.com/metasfresh/metasfresh/issues/11474) Boilerplate variables might fail silently
  * [#11479](https://github.com/metasfresh/metasfresh/issues/11479) Fix process of setting the parent of an account
  * [#11494](https://github.com/metasfresh/metasfresh/issues/11494) Another Regional Manager DownLine Export Problem
  * [#11496](https://github.com/metasfresh/metasfresh/issues/11496) Only change org of order from new partner if role has access to it
  * [#11512](https://github.com/metasfresh/metasfresh/pull/11512) Create quotation from project fixes
  * [#11517](https://github.com/metasfresh/metasfresh/pull/11517) `5599030_sys_valrule_Fresh_SalesPriceList_Version_of_BPartner_add_depends_on_C_BPartner.sql`
  * [#11549](https://github.com/metasfresh/metasfresh/issues/11549) Allow importing 0.00 bank statement lines
  * [#11560](https://github.com/metasfresh/metasfresh/issues/11560) Show gross weight as qty CU for HU editor lines with weight UOMs
  * [#11565](https://github.com/metasfresh/metasfresh/issues/11565) "Issue CUs from source HUs" not working in case source HUs include a HU which is CU on LU
  * [#11567](https://github.com/metasfresh/metasfresh/issues/11567) Have the supportOpenRecord set correctly by the BE for product proposal
  * [#11569](https://github.com/metasfresh/metasfresh/issues/11569) Consider the `supportOpenRecord` for the products proposal table
  * [#11602](https://github.com/metasfresh/metasfresh/issues/11602) Caption not correctly set when filtering by label in the Filter component
  * [#11609](https://github.com/metasfresh/metasfresh/pull/11609) Fix subheader actions

# metasfresh 5.170
## Features
* metasfresh
  * [#11051](https://github.com/metasfresh/metasfresh/issues/11051) API Audit
  * [#11129](https://github.com/metasfresh/metasfresh/issues/11129) Make "Add/Remove Credit Stop Status" available in BPartner window
  * [#11130](https://github.com/metasfresh/metasfresh/issues/11130) Overhaul the `C_Tax` business logic for OSS
  * [#11131](https://github.com/metasfresh/metasfresh/issues/11131) Article Statistics Improvements
  * [#11140](https://github.com/metasfresh/metasfresh/pull/11140) Lookup widget: "More results" indicator
  * [#11141](https://github.com/metasfresh/metasfresh/issues/11141) Create Tool for for invoice-tax QA
  * [#11145](https://github.com/metasfresh/metasfresh/issues/11145) Implement the possibility to add a footer image in a dynamic way
  * [#11153](https://github.com/metasfresh/metasfresh/issues/11153) Set `InvoiceCandidate` `DocTypeId`
  * [#11156](https://github.com/metasfresh/metasfresh/pull/11156) `C_BP_BankAccount_Acct.Payment_WriteOff_Acct`
  * [#11166](https://github.com/metasfresh/metasfresh/issues/11166) Display field `IsAutoAllocateAvailableAmt` in Payment window
  * [#11172](https://github.com/metasfresh/metasfresh/issues/11172) Budget Payment WriteOff process
  * [#11177](https://github.com/metasfresh/metasfresh/issues/11177) Report: List of qtybook of Products for a given date
  * [#11184](https://github.com/metasfresh/metasfresh/issues/11184) Introduce Error Message for invoicing error
  * [#11190](https://github.com/metasfresh/metasfresh/issues/11190) Fix `BusinessPartnerAccountSheetReport` to take payments in consideration
  * [#11192](https://github.com/metasfresh/metasfresh/issues/11192) Introduce `C_Greeting.GreetingStandardType`
  * [#11195](https://github.com/metasfresh/metasfresh/issues/11195) New BPartner window: Multiple contacts
  * [#11202](https://github.com/metasfresh/metasfresh/issues/11202) Attachment REST-API
  * [#11208](https://github.com/metasfresh/metasfresh/issues/11208) Create Shop Category Table and window
  * [#11219](https://github.com/metasfresh/metasfresh/issues/11219) New Shop Columns in `M_Product` Table
  * [#11220](https://github.com/metasfresh/metasfresh/issues/11220) `M_Product` Exclude from Flatrate Conditions
  * [#11227](https://github.com/metasfresh/metasfresh/issues/11227) Bank Account Invoice Auto Allocation Rules
  * [#11232](https://github.com/metasfresh/metasfresh/issues/11232) Update EU country table
  * [#11236](https://github.com/metasfresh/metasfresh/issues/11236) DB-Function to scramble sensitive metasfresh data
  * [#11240](https://github.com/metasfresh/metasfresh/issues/11240) API Audit - Log record references
  * [#11241](https://github.com/metasfresh/metasfresh/issues/11241) Exclude from Commission based on `DocType`
  * [#11242](https://github.com/metasfresh/metasfresh/pull/11242) Add websocket connection to the modal
  * [#11244](https://github.com/metasfresh/metasfresh/issues/11244) Attributes can be configured to be always updatable in HU
  * [#11252](https://github.com/metasfresh/metasfresh/pull/11252) Introduce micrometer.io
  * [#11253](https://github.com/metasfresh/metasfresh/pull/11253) metasfresh-orgs: order batch entry - explode compensation groups
  * [#11259](https://github.com/metasfresh/metasfresh/issues/11259) Implement: Read ESR QR Code of Vendor Invoices
  * [#11260](https://github.com/metasfresh/metasfresh/pull/11260) REST endpoint: get HU by SerialNo
  * [#11262](https://github.com/metasfresh/metasfresh/issues/11262) Alberta - Sync BPartners
  * [#11267](https://github.com/metasfresh/metasfresh/issues/11267) Transform Product Attribute set, ASI into Flexible Masterdata recording
  * [#11268](https://github.com/metasfresh/metasfresh/issues/11268) Introduce Contact Attributes
  * [#11271](https://github.com/metasfresh/metasfresh/pull/11271) Create API EP for Out-Of-Stock Notice
  * [#11277](https://github.com/metasfresh/metasfresh/issues/11277) Introduce `C_BPartner_Attribute2`, `C_BPartner_Attribute3`, `C_BPartner_Attribute4`, `C_BPartner_Attribute5` Tables and Ref Lists
  * [#11281](https://github.com/metasfresh/metasfresh/issues/11281) Make the reading of QR code user friendly
  * [#11292](https://github.com/metasfresh/metasfresh/issues/11292) Missing Manufacturing Activity in Manufacturing Workflow
  * [#11300](https://github.com/metasfresh/metasfresh/issues/11300) New `ExcludeFromPromotions` and Referrer columns in `C_BPartnert_QuickInput` Table
  * [#11312](https://github.com/metasfresh/metasfresh/issues/11312) Implement `BPartnerNameAndGreetingStrategy` for membership contacts
  * [#11316](https://github.com/metasfresh/metasfresh/issues/11316) Introduce `C_CompensationGroup_Schema_Category` table
  * [#11318](https://github.com/metasfresh/metasfresh/pull/11318) `AD_Process.IsFormatExcelFile`
  * [#11324](https://github.com/metasfresh/metasfresh/issues/11324) Fetch VAT Notice in Documents from `C_Tax`
  * [#11326](https://github.com/metasfresh/metasfresh/pull/11326) `GroupTemplateRepository`: allow group templates without compensation lines
  * [#11329](https://github.com/metasfresh/metasfresh/pull/11329) Authenticate when pulling from dockerhub with jib
  * [#11334](https://github.com/metasfresh/metasfresh/issues/11334) On BPartner Search Assistant, show associated contact names, not bpartner names
  * [#11340](https://github.com/metasfresh/metasfresh/pull/11340) Order: copy Org from BPartner (if configured)
  * [#11341](https://github.com/metasfresh/metasfresh/issues/11341) Invoke `ExternalSystem` via RabbitMQ
  * [#11343](https://github.com/metasfresh/metasfresh/issues/11343) New doctype mediated PO
  * [#11346](https://github.com/metasfresh/metasfresh/pull/11346) Master Alberta runtime parameters
  * [#11350](https://github.com/metasfresh/metasfresh/issues/11350) Introduce "External-System-URL"
  * [#11351](https://github.com/metasfresh/metasfresh/pull/11351) Handling units editor: show barcode filter inline
  * [#11353](https://github.com/metasfresh/metasfresh/issues/11353) Allow single bpartner filter field to filter by name, value and city
  * [#11356](https://github.com/metasfresh/metasfresh/issues/11356) Effort Issues Budget don't update when bud label changes
  * [#11358](https://github.com/metasfresh/metasfresh/issues/11358) Add new column `C_BPartner.C_Campaign_ID` and `C_BPartner_QuickInput.C_Campaign_ID`
  * [#11362](https://github.com/metasfresh/metasfresh/issues/11362) Org Change: Use Compensation Group Schemas to determine which are subscriptions in target org
  * [#11364](https://github.com/metasfresh/metasfresh/issues/11364) Order window: Add missing trl in `de_DE`/`de_CH`
  * [#11366](https://github.com/metasfresh/metasfresh/issues/11366) Add GLN to address field for documents
  * [#11371](https://github.com/metasfresh/metasfresh/issues/11371) WebUI frontend: redesign the dashboard target indicators
  * [#11374](https://github.com/metasfresh/metasfresh/issues/11374) Extend Country display sequence to allow building addresses with Partner's greeting
  * [#11375](https://github.com/metasfresh/metasfresh/pull/11375) Implement SQL KPIs
  * [#11378](https://github.com/metasfresh/metasfresh/issues/11378) Doc-Outbound-Log - Distinguish between `DocumentNo` and `FileName`
  * [#11380](https://github.com/metasfresh/metasfresh/issues/11380) Create Invoice Subtab in BPartner Window
  * [#11381](https://github.com/metasfresh/metasfresh/issues/11381) WebUI frontend: show Details link to target indicators
  * [#11386](https://github.com/metasfresh/metasfresh/issues/11386) WebUI frontend: show last computed text to target indicators
  * [#11387](https://github.com/metasfresh/metasfresh/issues/11387) Implement QR report for dunning
  * [#11398](https://github.com/metasfresh/metasfresh/issues/11398) Update babel* packages
  * [#11405](https://github.com/metasfresh/metasfresh/issues/11405) Bank's routing number shall not be mandatory
  * [#11408](https://github.com/metasfresh/metasfresh/pull/11408) `CopyAttributesFromBOMLineGenerator`
  * [#11409](https://github.com/metasfresh/metasfresh/issues/11409) Extend `edi_desadvpack_sscc_label`
  * [#11412](https://github.com/metasfresh/metasfresh/issues/11412) API-Audit - Notify user \*group\*
  * [#11416](https://github.com/metasfresh/metasfresh/issues/11416) Remove bidirectional relation type
  * [#11417](https://github.com/metasfresh/metasfresh/issues/11417) Request Window changes
  * [#11426](https://github.com/metasfresh/metasfresh/issues/11426) Product attachments should be visible, even if attached to parent products
  * [#11428](https://github.com/metasfresh/metasfresh/issues/11428) Add Postal Filter Converter for the BPartner Export
  * [#11429](https://github.com/metasfresh/metasfresh/issues/11429) Create a Label for Finished goods report from HU Editor
  * [#11440](https://github.com/metasfresh/metasfresh/issues/11440) Effort-issue window - indicate if parent is already invoiced
  * [#11454](https://github.com/metasfresh/metasfresh/pull/11454) Partial cost recalculation DB function
  * [#11467](https://github.com/metasfresh/metasfresh/issues/11467) Send also product category to Alberta

## Fixes
* metasfresh
  * [#11135](https://github.com/metasfresh/metasfresh/issues/11135) Invoice Rule `OrderCompletelyDelivered` should work with non-item-products
  * [#11137](https://github.com/metasfresh/metasfresh/issues/11137) Inventory UOM problem - Count items are not created
  * [#11169](https://github.com/metasfresh/metasfresh/issues/11169) Frontend should follow `IncludedTabsInfo` `allowCreateNew` and `allowDelete` props
  * [#11174](https://github.com/metasfresh/metasfresh/pull/11174) Prevent group with no value from incorrectly matching groups with an actual value
  * [#11193](https://github.com/metasfresh/metasfresh/pull/11193) Fix Kanban board
  * [#11206](https://github.com/metasfresh/metasfresh/pull/11206) `ShipmentScheduleUpdater`: Fix bug where `qtyToDeliver` was wrong
  * [#11211](https://github.com/metasfresh/metasfresh/issues/11211) Zoom into BPartner opens BPartner Info window
  * [#11216](https://github.com/metasfresh/metasfresh/issues/11216) Frontend - Kanban board: refresh the "Add cards" view on websocket event
  * [#11217](https://github.com/metasfresh/metasfresh/pull/11217) `ShipmentScheduleEnqueuer` - directly close the lock when done
  * [#11245](https://github.com/metasfresh/metasfresh/issues/11245) NPE when closing purchase order that has no receipt schedules yet
  * [#11248](https://github.com/metasfresh/metasfresh/issues/11248) CU label does not work properly in certain cases
  * [#11257](https://github.com/metasfresh/metasfresh/issues/11257) WebUI frontend: select order lines, ALT-Y, ENTER does not work
  * [#11258](https://github.com/metasfresh/metasfresh/issues/11258) Stop unnecessary request from widgets
  * [#11285](https://github.com/metasfresh/metasfresh/issues/11285) Active tab not refreshed on ws event
  * [#11305](https://github.com/metasfresh/metasfresh/issues/11305) 401 from the backend after updating row/using barcode search
  * [#11321](https://github.com/metasfresh/metasfresh/pull/11321) Master adapt v2 routes
  * [#11337](https://github.com/metasfresh/metasfresh/pull/11337) `BPartnerQuickInputService.createBPartnerFromTemplate`: consider Phone and email
  * [#11338](https://github.com/metasfresh/metasfresh/issues/11338) Update inline tab's valid status on PATCH
  * [#11344](https://github.com/metasfresh/metasfresh/issues/11344) In purchase order document the price precision is not respected
  * [#11360](https://github.com/metasfresh/metasfresh/issues/11360) Prevent reversed credit memo from making invoice candidate invoiceable again
  * [#11368](https://github.com/metasfresh/metasfresh/issues/11368) Error from Link when creating a new KPI Dashboard
  * [#11407](https://github.com/metasfresh/metasfresh/issues/11407) Fix & Tweak `C_Commission_RegionalManagerRevenue_v`
  * [#11432](https://github.com/metasfresh/metasfresh/issues/11432) Letter creation is not working anymore
  * [#11438](https://github.com/metasfresh/metasfresh/issues/11438) `01. Suchauswahl abw. Werte setzen` should either set both bpartner & location, or none at all
  * [#11442](https://github.com/metasfresh/metasfresh/issues/11442) Payment Discount ("Skonto") not allocated when using Prepay Order
  * [#11444](https://github.com/metasfresh/metasfresh/issues/11444) Investigate/fix the issue with the loading not showing while filtering is pending
  * [#11450](https://github.com/metasfresh/metasfresh/issues/11450) Problem with computing storage attribute keys
  * [#11451](https://github.com/metasfresh/metasfresh/pull/11451) Fix an error with receipt schedule and manufacturing EP
  * [#11462](https://github.com/metasfresh/metasfresh/pull/11462) Avoid OOME from micromenter.io

# metasfresh 5.169
## Features
* metasfresh
  * [#11024](https://github.com/metasfresh/metasfresh/issues/11024) Add EDI fields to Bpartner window
  * [#11069](https://github.com/metasfresh/metasfresh/issues/11069) Budget Window adjustmenst (invoiceable effort)
  * [#11079](https://github.com/metasfresh/metasfresh/issues/11079) Shopware: BPartner sync advice
  * [#11084](https://github.com/metasfresh/metasfresh/issues/11084) BPartner Rest V2: support external reference version
  * [#11088](https://github.com/metasfresh/metasfresh/issues/11088) Garantiezeit 60 Monate hinzufügen
  * [#11094](https://github.com/metasfresh/metasfresh/issues/11094) Funktion für Erfassung Initial-CostPrice
  * [#11098](https://github.com/metasfresh/metasfresh/issues/11098) Product Rest V2: support external reference version
  * [#11067](https://github.com/metasfresh/metasfresh/issues/11067) Shopware: shipper & shipping costs
  * [#11107](https://github.com/metasfresh/metasfresh/issues/11107) Geschäftspartner: Dropdown Menü für Incoterms
  * [#11112](https://github.com/metasfresh/metasfresh/issues/11112) Update the packages flagged as highly vulnerable
  * [#11119](https://github.com/metasfresh/metasfresh/issues/11119) Create Sales/Purchase Price List action
  * [#11126](https://github.com/metasfresh/metasfresh/issues/11126) When creating a counter document, the original document needs to also reference it
  * [#11164](https://github.com/metasfresh/metasfresh/issues/11164) Add Customer Retention Initial Threshold
  * [#11169](https://github.com/metasfresh/metasfresh/issues/11169) Frontend should follow IncludedTabsInfo allowCreateNew and allowDelete props
  * [#11101](https://github.com/metasfresh/metasfresh/issues/11101) Use EAN128/GS1-128 barcode in sscc label
  * [#11134](https://github.com/metasfresh/metasfresh/issues/11134) Extend Alberta Masterdata Sync
  * [#11077](https://github.com/metasfresh/metasfresh/pull/11077) working on a cucumber sales order and commission test
  * [#11090](https://github.com/metasfresh/metasfresh/pull/11090) BankStatementDocumentHandler.completeIt: consider already assigned payments first
  * [#11093](https://github.com/metasfresh/metasfresh/pull/11093) add field to display the child-issues's invoicable effort
  * [#11103](https://github.com/metasfresh/metasfresh/pull/11103) inherit related processes from base window
  * [#11113](https://github.com/metasfresh/metasfresh/pull/11113) AD_Column.isexcludefromzoomtargets initialize
  * [#11114](https://github.com/metasfresh/metasfresh/pull/11114) modernize C_OrderMFGWarehouse MIs
  * [#11122](https://github.com/metasfresh/metasfresh/pull/11122) WebuiDocumentPrintService: consider document's doc outbound recipient when determining the flavor

## Fixes
* metasfresh
  * [#11070](https://github.com/metasfresh/metasfresh/issues/11070) Investigate build issue introduced by prettier
  * [#11082](https://github.com/metasfresh/metasfresh/issues/11082) Umsatzreport Geschäftspartner Woche
  * [#11091](https://github.com/metasfresh/metasfresh/issues/11091) Leergut-Rücknahme ergibt Fehlermeldung
  * [#11096](https://github.com/metasfresh/metasfresh/issues/11096) Organisation window is not working properly
  * [#11118](https://github.com/metasfresh/metasfresh/issues/11118) "Qty shall be greather than zero" error when creating orderline with batch entry
  * [#11171](https://github.com/metasfresh/metasfresh/issues/11171) sync M_warehouse.c_bpartner_location_id to c_bpartner_location.c_bpartner_location_id
  * [#11032](https://github.com/metasfresh/metasfresh/pull/11032) Fix two inventory related problems
  * [#11092](https://github.com/metasfresh/metasfresh/pull/11092) related documents fixes
  * [#11111](https://github.com/metasfresh/metasfresh/pull/11111) Shipment-REST-API - avoid QtyToDeliver_Override race condition
  * [#11157](https://github.com/metasfresh/metasfresh/pull/11157) Fix sitemap alignment
  * [#11144](https://github.com/metasfresh/metasfresh/issues/11144) Debug & fix manual discount not working in sales order line

# metasfresh 5.168
## Features
* metasfresh
  * [#10860](https://github.com/metasfresh/metasfresh/issues/10860) Refactor the rest of the direct usages of RawWidget
  * [#11016](https://github.com/metasfresh/metasfresh/issues/11016) `Alberta_PrescriptionRequest` Tables and Window
  * [#11026](https://github.com/metasfresh/metasfresh/issues/11026) Provisionsübersicht Window Update
  * [#11028](https://github.com/metasfresh/metasfresh/issues/11028) Create default `invoiceRule` Configuration
  * [#11036](https://github.com/metasfresh/metasfresh/issues/11036) Do not allow to create duplicate sales partner code
  * [#11039](https://github.com/metasfresh/metasfresh/pull/11039) `DocOutbound` shall consider `IsInvoiceEmailEnabled` flag
  * [#11041](https://github.com/metasfresh/metasfresh/issues/11041) External system "Other" setup
  * [#11043](https://github.com/metasfresh/metasfresh/pull/11043) Build improvements
  * [#11045](https://github.com/metasfresh/metasfresh/pull/11045) Replace `FactAcctLogWorkpackageProcessor` with `FactAcctLogDBTableWatcher`
  * [#11048](https://github.com/metasfresh/metasfresh/issues/11048) `C_Tax` window Changes
  * [#11054](https://github.com/metasfresh/metasfresh/issues/11054) Create `C_Fiscal_Representation` table, tab and model
  * [#11062](https://github.com/metasfresh/metasfresh/issues/11062) Add "Available For Sales" stock info to `productLookup` and make it the default look-up method
  * [#11064](https://github.com/metasfresh/metasfresh/issues/11064) Add organization in charge to postal

## Fixes
* metasfresh
  * [#10655](https://github.com/metasfresh/metasfresh/issues/10655) Pricesystem of contract term not considered correctly
  * [#10931](https://github.com/metasfresh/metasfresh/issues/10931) Filter default values are ignored
  * [#11014](https://github.com/metasfresh/metasfresh/issues/11014) Check automated e2e tests mid April
  * [#11031](https://github.com/metasfresh/metasfresh/pull/11031) Prevent creating OL candidates with stocked products that are flagged as main product in compensation group
  * [#11044](https://github.com/metasfresh/metasfresh/pull/11044) Invoice-Line: Update `PriceActual` as user edits `PriceEntered` and Discount
  * [#11049](https://github.com/metasfresh/metasfresh/issues/11049) Beginning of May e2e checks
  * [#11050](https://github.com/metasfresh/metasfresh/issues/11050) "Not Found" error when using "Create purchase orders" action for sales orderline

# metasfresh 5.167
## Features
* metasfresh
  * [#10955](https://github.com/metasfresh/metasfresh/issues/10955) Update Elasticsearch in our stack
  * [#10990](https://github.com/metasfresh/metasfresh/issues/10990) Support for a process triggered by model interceptor
  * [#10999](https://github.com/metasfresh/metasfresh/issues/10999) Support for a process triggered by model interceptor - frontend
  * [#11000](https://github.com/metasfresh/metasfresh/issues/11000) Support zoom for labels
  * [#11001](https://github.com/metasfresh/metasfresh/pull/11001) Elasticsearch docker integration
  * [#11008](https://github.com/metasfresh/metasfresh/issues/11008) Add TRL for the Repair Workflows
  * [#11011](https://github.com/metasfresh/metasfresh/pull/11011) Allow webAPI to schedule a workpackage and wait for it to be done

## Fixes
* metasfresh
  * [#10899](https://github.com/metasfresh/metasfresh/pull/10899) Elasticsearch / dashboard fix
  * [#11007](https://github.com/metasfresh/metasfresh/issues/11007) Uncaught error in promise when setting Business Partner

# metasfresh 5.166
## Features
* metasfresh
  * [#10912](https://github.com/metasfresh/metasfresh/issues/10912) Pimp the menu structure & UI
  * [#10947](https://github.com/metasfresh/metasfresh/issues/10947) Display `ApprovalForInvoicing` in invoice candidates (single view)
  * [#10958](https://github.com/metasfresh/metasfresh/issues/10958) "Add New" not present in the Warehouse NEW
  * [#10964](https://github.com/metasfresh/metasfresh/issues/10964) End of Year GL Journal
  * [#10975](https://github.com/metasfresh/metasfresh/pull/10975) `PPOrderLineRow.lineStatusColor`
  * [#10979](https://github.com/metasfresh/metasfresh/issues/10979) Option for keeping price 0 when copying price lists
  * [#10980](https://github.com/metasfresh/metasfresh/pull/10980) Bump up guava version and remove obsolete log4j dependency
  * [#10985](https://github.com/metasfresh/metasfresh/issues/10985) Email in orders' doc outbound documents
  * [#10987](https://github.com/metasfresh/metasfresh/pull/10987) Alberta orders: always sync delivery address before importing
  * [#10993](https://github.com/metasfresh/metasfresh/pull/10993) Price Comparation report performance improvements
  * [#10997](https://github.com/metasfresh/metasfresh/issues/10997) Import Shopware `OL_Cands`

## Fixes
* metasfresh
  * [#10931](https://github.com/metasfresh/metasfresh/issues/10931) Filter default values are ignored
  * [#10953](https://github.com/metasfresh/metasfresh/issues/10953) Fix dependency in the frontend packages
  * [#10974](https://github.com/metasfresh/metasfresh/pull/10974) Bidirectional sync between `AD_User` and procurement user
  * [#10976](https://github.com/metasfresh/metasfresh/pull/10976) `ProductBOMDAO.getDefaultBOM`, consider `MakeToOrder` too when checking for default BOM
  * [#10981](https://github.com/metasfresh/metasfresh/issues/10981) procurement-webui-frontend cannot be started on localhost
  * [#10986](https://github.com/metasfresh/metasfresh/pull/10986) Don't check the last HU Trx for internal use inventory
  * [#10994](https://github.com/metasfresh/metasfresh/pull/10994) Fix procurement WebUI RfQ import

# metasfresh 5.165
## Features
* metasfresh
  * [#10700](https://github.com/metasfresh/metasfresh/issues/10700) Forced Org Switch process
  * [#10841](https://github.com/metasfresh/metasfresh/issues/10841) Add `PurchaseOrderCandidate` REST controller
  * [#10866](https://github.com/metasfresh/metasfresh/issues/10866) Allow deleting `C_BPartners` that have locations, etc.
  * [#10890](https://github.com/metasfresh/metasfresh/issues/10890) Adapt FE formatting of the highlighted string with the order provided by the BE
  * [#10896](https://github.com/metasfresh/metasfresh/pull/10896) Improve `POInfo` loading
  * [#10897](https://github.com/metasfresh/metasfresh/issues/10897) Prevent setting Sales rep with the same value as bpartner
  * [#10898](https://github.com/metasfresh/metasfresh/pull/10898) Fail if the `AD_Column`'s or `AD_Field`'s lookup is not correctly defined
  * [#10902](https://github.com/metasfresh/metasfresh/issues/10902) Rabatte Export
  * [#10903](https://github.com/metasfresh/metasfresh/issues/10903) Check automated e2e tests end of March
  * [#10904](https://github.com/metasfresh/metasfresh/issues/10904) Retrieve sales orders from Alberta
  * [#10919](https://github.com/metasfresh/metasfresh/pull/10919) `WindowRestController.getDocumentFieldZoomInto`: Use override window if any
  * [#10921](https://github.com/metasfresh/metasfresh/issues/10921) Provide `Setup_Place_No` in INVOIC-XML
  * [#10924](https://github.com/metasfresh/metasfresh/issues/10924) Implement dynamic product label
  * [#10928](https://github.com/metasfresh/metasfresh/issues/10928) Allow specifying compensation groups from orderline candidates
  * [#10933](https://github.com/metasfresh/metasfresh/issues/10933) Extend process `de.metas.ui.web.pricing.process.M_DiscountSchemaBreak_CopyToSelectedSchema_Product`
  * [#10934](https://github.com/metasfresh/metasfresh/pull/10934) WebUI Dashboard: Websocket notifications + fixes
  * [#10935](https://github.com/metasfresh/metasfresh/pull/10935) Introduce `JsonRequestIssueToManufacturingOrder.process` flag
  * [#10945](https://github.com/metasfresh/metasfresh/issues/10945) Upgrade Cypress & fix legacy dependencies
  * [#10946](https://github.com/metasfresh/metasfresh/pull/10946) Masterdata bpartner cucumber
  * [#10952](https://github.com/metasfresh/metasfresh/pull/10952) New material withdrawal process (Materialentnahme)
  * [#10962](https://github.com/metasfresh/metasfresh/issues/10962) Add specification column to `pp_wf_node_product` & `pp_order_node_product`

## Fixes
* metasfresh
  * [#10402](https://github.com/metasfresh/metasfresh/pull/10402) Create Sales Order from Quotation error
  * [#10831](https://github.com/metasfresh/metasfresh/issues/10831) Update frontend vulnerable packages
  * [#10881](https://github.com/metasfresh/metasfresh/issues/10881) When sitemap is opened the menu entries (quick and sitemap entries) don't start processes/actions anymore
  * [#10916](https://github.com/metasfresh/metasfresh/pull/10916) Fix and optimize payment allocation for huge number of invoices
  * [#10925](https://github.com/metasfresh/metasfresh/issues/10925) If URL contains a `viewId`, refreshing after login in another tab causes white screen (after timeout logout)
  * [#10931](https://github.com/metasfresh/metasfresh/issues/10931) Filter default values are ignored
  * [#10939](https://github.com/metasfresh/metasfresh/issues/10939) Minor printing-related improvements
  * [#10944](https://github.com/metasfresh/metasfresh/issues/10944) When looking up BPartners from the REST-API to update, also check for Org=`*`

# metasfresh 5.164
## Features
* metasfresh
  * [#10704](https://github.com/metasfresh/metasfresh/issues/10704) Debitor/Creditor in Bank Statement import
  * [#10774](https://github.com/metasfresh/metasfresh/pull/10774) Add CostPrice component
  * [#10784](https://github.com/metasfresh/metasfresh/issues/10784) Overhaul BPartner-ExternalReference in API-v2
  * [#10796](https://github.com/metasfresh/metasfresh/issues/10796) Store Alberta Article materdata for `M_Products`
  * [#10807](https://github.com/metasfresh/metasfresh/pull/10807) Consider HU's warehouse and bpartner when filtering by barcode/sscc18
  * [#10811](https://github.com/metasfresh/metasfresh/issues/10811) Add Manufacturing Activity products tab
  * [#10818](https://github.com/metasfresh/metasfresh/issues/10818) Push products to Alberta
  * [#10822](https://github.com/metasfresh/metasfresh/pull/10822) `EDI_Desadv_GenerateSSCCLabels`: introduce `IsDefault` param
  * [#10824](https://github.com/metasfresh/metasfresh/pull/10824) `CellValues.toCellValue`: Fix conversions
  * [#10825](https://github.com/metasfresh/metasfresh/issues/10825) Upsert Products V2 REST API
  * [#10834](https://github.com/metasfresh/metasfresh/pull/10834) `HUsToReturn_CreateShippedHU`; `M_InOutLine.IsWarrantyCase`
  * [#10842](https://github.com/metasfresh/metasfresh/issues/10842) Upgrade react-transition-group
  * [#10847](https://github.com/metasfresh/metasfresh/issues/10847) Upsert Prices REST
  * [#10850](https://github.com/metasfresh/metasfresh/pull/10850) Creating Sales Orders: Don't set salesrep if equal to buyer
  * [#10851](https://github.com/metasfresh/metasfresh/issues/10851) Don't show the RootFolder of Role Menu
  * [#10868](https://github.com/metasfresh/metasfresh/pull/10868) Master spring boot 2
  * [#10891](https://github.com/metasfresh/metasfresh/issues/10891) Order of fields within the Alberta `inlineTab` element

## Fixes
* metasfresh
  * [#9845](https://github.com/metasfresh/metasfresh/issues/9845) Warning during compile time
  * [#10785](https://github.com/metasfresh/metasfresh/issues/10785) `BPartnerLocation` data should not default to locations from other countries
  * [#10810](https://github.com/metasfresh/metasfresh/pull/10810) OrderBL: when fetching the Order PricingSystem use the order's BPartner
  * [#10817](https://github.com/metasfresh/metasfresh/issues/10817) Make sure that there is no npm dep package blocking installation
  * [#10826](https://github.com/metasfresh/metasfresh/issues/10826) Investigate failing tests for period - end of Feb 2021-March 15, 2021
  * [#10829](https://github.com/metasfresh/metasfresh/pull/10829) `R_Request`: Grant permissions to creator
  * [#10832](https://github.com/metasfresh/metasfresh/issues/10832) Possible "Duplicate Key Error" when loading records with data entry tabs
  * [#10843](https://github.com/metasfresh/metasfresh/issues/10843) ESR Import Error for new QR Invoice
  * [#10845](https://github.com/metasfresh/metasfresh/pull/10845) WebUI: Fix HU view filtering and invalidation
  * [#10846](https://github.com/metasfresh/metasfresh/issues/10846) Make `AD_Column` `C_Customer_Retention.CustomerRetention` updatable
  * [#10848](https://github.com/metasfresh/metasfresh/pull/10848) Return even inactive `C_BPartner_Locations` at many places
  * [#10854](https://github.com/metasfresh/metasfresh/pull/10854) `PPOrderLinesViewDataLoader`: Consider only Active source HUs
  * [#10861](https://github.com/metasfresh/metasfresh/issues/10861) Procurement planning - orders cannot be triggered
  * [#10864](https://github.com/metasfresh/metasfresh/issues/10864) Clear filter after searching an item (not in db) seems it cannot be done
  * [#10869](https://github.com/metasfresh/metasfresh/pull/10869) Fix `HUsToReturn_CreateShippedHU`
  * [#10873](https://github.com/metasfresh/metasfresh/issues/10873) Cookie problem
  * [#10876](https://github.com/metasfresh/metasfresh/issues/10876) Ablaufsteuerung Refresh `MV_Fact_Acct_Sum` does not do what it shall
  * [#10889](https://github.com/metasfresh/metasfresh/pull/10889) Only consider commission contracts that have the trigger-document's org

# metasfresh 5.163
## Features
* metasfresh
  * [#10748](https://github.com/metasfresh/metasfresh/issues/10748) Improve and extend copy discount lines on product
  * [#10756](https://github.com/metasfresh/metasfresh/issues/10756) Precision in sync with BE
  * [#10766](https://github.com/metasfresh/metasfresh/issues/10766) Extend external system status window
  * [#10767](https://github.com/metasfresh/metasfresh/issues/10767) Token-based authentication
  * [#10769](https://github.com/metasfresh/metasfresh/issues/10769) Business Partner Advanced Search
  * [#10775](https://github.com/metasfresh/metasfresh/issues/10775) Alberta dedicated Camel route: sync Pharmacy
  * [#10778](https://github.com/metasfresh/metasfresh/issues/10778) Manufacturing Order improvement: FiFo for reversed issue cases, report error
  * [#10789](https://github.com/metasfresh/metasfresh/issues/10789) Clone Product with `M_Product_Acct` records
  * [#10790](https://github.com/metasfresh/metasfresh/issues/10790) Service Repair Scripts
  * [#10793](https://github.com/metasfresh/metasfresh/issues/10793) Display `PP_Order` attribute in HU only if in attribute set
  * [#10798](https://github.com/metasfresh/metasfresh/pull/10798) Picking Terminal 1: Search by Barcode
  * [#10805](https://github.com/metasfresh/metasfresh/issues/10805) Add a print format for Customs Invoice

## Fixes
* metasfresh
  * [#10765](https://github.com/metasfresh/metasfresh/issues/10765) Invalid `viewId`: null on payment allocations
  * [#10800](https://github.com/metasfresh/metasfresh/pull/10800) `EDI_Desadv_GenerateSSCCLabels` fixes

# metasfresh 5.162
## Features
* metasfresh
  * [#10541](https://github.com/metasfresh/metasfresh/issues/10541) Process to reconstruct commission data from `C_BPartner.C_BPartner_SalesRep_ID`'s changelog
  * [#10565](https://github.com/metasfresh/metasfresh/pull/10565) WebUI: Zoom Into shall open the right window
  * [#10568](https://github.com/metasfresh/metasfresh/issues/10568) Add Org filter for intratrade and intracommunity reports
  * [#10648](https://github.com/metasfresh/metasfresh/issues/10648) Add guarantee time in months
  * [#10653](https://github.com/metasfresh/metasfresh/pull/10653) Allow sending email from WebUI without SMTP-credentials set in `AD_User`
  * [#10661](https://github.com/metasfresh/metasfresh/issues/10661) New `ProblemCode` field in `PP_Order` table
  * [#10664](https://github.com/metasfresh/metasfresh/pull/10664) Show `SerialNo` attribute + translation
  * [#10666](https://github.com/metasfresh/metasfresh/issues/10666) Tune material cockpit default settings
  * [#10667](https://github.com/metasfresh/metasfresh/issues/10667) Create `AD_Zebra_Config` Table
  * [#10669](https://github.com/metasfresh/metasfresh/pull/10669) `CreatePOFromSOsAggregator`: improve error message; `QueryStatisticsLogger`: fix it
  * [#10670](https://github.com/metasfresh/metasfresh/issues/10670) Add Accounting date to windows that support it
  * [#10674](https://github.com/metasfresh/metasfresh/pull/10674) `AD_User_Record_Access_UpdateFrom_BPartnerHierarchy`: Use the new `C_BPartner.c_bpartner_salesrep_id` hierarchy
  * [#10687](https://github.com/metasfresh/metasfresh/issues/10687) External System Tweaks
  * [#10691](https://github.com/metasfresh/metasfresh/issues/10691) Create Window External system log
  * [#10693](https://github.com/metasfresh/metasfresh/issues/10693) Alberta: sync payer
  * [#10696](https://github.com/metasfresh/metasfresh/issues/10696) `AD_PInstance_Log` Rest Endpoint
  * [#10697](https://github.com/metasfresh/metasfresh/pull/10697) Improve performance of material receipt dispo for large DBs
  * [#10702](https://github.com/metasfresh/metasfresh/pull/10702) Editing packing item override option to be changed
  * [#10704](https://github.com/metasfresh/metasfresh/issues/10704) Debitor/Creditor in Bank Statement import
  * [#10705](https://github.com/metasfresh/metasfresh/issues/10705) Allow creating commission-deed for purchase done by salesrep themselves
  * [#10718](https://github.com/metasfresh/metasfresh/issues/10718) Add Frame Agreement and Order Call SO doc types
  * [#10724](https://github.com/metasfresh/metasfresh/issues/10724) Shopware dedicated camel route
  * [#10729](https://github.com/metasfresh/metasfresh/pull/10729) stepcom-orderss-edi - guard against prices with too many digits behind the decimal point
  * [#10736](https://github.com/metasfresh/metasfresh/issues/10736) Feld Dropdown Produktfenster "Vegan/Vegetarisch"
  * [#10739](https://github.com/metasfresh/metasfresh/pull/10739) `ADW_Window.Overrides_Window_ID` improvements
  * [#10741](https://github.com/metasfresh/metasfresh/issues/10741) Customize Window Payment Selection
  * [#10743](https://github.com/metasfresh/metasfresh/pull/10743) `DeliveredDataLoader`: fallback to stocking UOM in case `C_InvoiceCandidate_InOutLine.C_UOM_ID` is not set
  * [#10749](https://github.com/metasfresh/metasfresh/issues/10749) Allow adding on non-stocked items to physical inventory
  * [#10759](https://github.com/metasfresh/metasfresh/pull/10759) Payment Allocation: Invoice Row - `IsPreparedForAllocation`
  * [#10760](https://github.com/metasfresh/metasfresh/issues/10760) Retrieve bpartner-masterdata from shopware6
  * [#10763](https://github.com/metasfresh/metasfresh/pull/10763) WebUI login with token

## Fixes
* metasfresh
  * [#10516](https://github.com/metasfresh/metasfresh/issues/10516) Don't update `CanBeExportedAfter` value if nothing changed
  * [#10647](https://github.com/metasfresh/metasfresh/pull/10647) Hotfix `OrderBL.setBill_User_ID`
  * [#10656](https://github.com/metasfresh/metasfresh/issues/10656) Inventory import when no `huAggregationType` is set
  * [#10681](https://github.com/metasfresh/metasfresh/issues/10681) Show Standard account from Org in 0 in balance sheet
  * [#10698](https://github.com/metasfresh/metasfresh/pull/10698) `DebugTraceSqlQueriesRestController`
  * [#10711](https://github.com/metasfresh/metasfresh/pull/10711) Don't remove the HU from view after moving it
  * [#10713](https://github.com/metasfresh/metasfresh/pull/10713) Avoid spring cyclic dep by introducing `RecordAccessRepository`
  * [#10717](https://github.com/metasfresh/metasfresh/pull/10717) Fix `paymentAllocatedAmt` in case of fixed conversion rate
  * [#10733](https://github.com/metasfresh/metasfresh/pull/10733) Restore old `C_Order_CreatePOFromSOs` process
  * [#10734](https://github.com/metasfresh/metasfresh/issues/10734) Issue CUs from Source HUs failing for different UOMs
  * [#10751](https://github.com/metasfresh/metasfresh/pull/10751) Hotfix allocation posting for APC invoices
  * [#10754](https://github.com/metasfresh/metasfresh/issues/10754) Camel-EDI: Number format improvement
  * [#10757](https://github.com/metasfresh/metasfresh/issues/10757) Update `M_ShipmentSchedule.CanBeExportedFrom` when changing export status

# metasfresh 5.161
## Features
* metasfresh
  * [#10249](https://github.com/metasfresh/metasfresh/issues/10249) Printing Options: WebUI frontend panel
  * [#10269](https://github.com/metasfresh/metasfresh/issues/10269) Possibility for Address & User input in Main view (not in subtab)
  * [#10275](https://github.com/metasfresh/metasfresh/issues/10275) Implement `AD_UI_Element.Inline_Tab_ID`
  * [#10389](https://github.com/metasfresh/metasfresh/issues/10389) Guarantee/Service Cases: Set `WarrantyStartDate` when shipping HUs
  * [#10393](https://github.com/metasfresh/metasfresh/issues/10393) Add 'Show Less' and 'Show More' `ad_messages`
  * [#10419](https://github.com/metasfresh/metasfresh/issues/10419) Create a function that should say if a country is in EU or not
  * [#10424](https://github.com/metasfresh/metasfresh/issues/10424) Service Orders: Kickstart Service/Repair Project window
  * [#10426](https://github.com/metasfresh/metasfresh/issues/10426) Only add `SerialNo` Attribute to Manufacturing
  * [#10432](https://github.com/metasfresh/metasfresh/pull/10432) Delete old swing classes
  * [#10438](https://github.com/metasfresh/metasfresh/issues/10438) Capture BOM components of a manufactured HU to be able to recall it after time
  * [#10446](https://github.com/metasfresh/metasfresh/issues/10446) Guarantee/Service Cases: Clone a Shipped/inactive HU
  * [#10448](https://github.com/metasfresh/metasfresh/issues/10448) Add a new invoice rule: Order Completely Delivered
  * [#10455](https://github.com/metasfresh/metasfresh/issues/10455) Add `PresetDateInvoiced`, `DateAcct`, `DateInvoiced` to default aggregation rule
  * [#10464](https://github.com/metasfresh/metasfresh/issues/10464) New procurement WebUI: Create a new spring boot/Maven project
  * [#10467](https://github.com/metasfresh/metasfresh/issues/10467) `m_product.isstocked` new parm in inventory lines creating processes
  * [#10478](https://github.com/metasfresh/metasfresh/issues/10478) Remove legacy jax-rs and jms code
  * [#10481](https://github.com/metasfresh/metasfresh/pull/10481) StepComXMLDesadvBean and CompuDataDesadvBean: don't remove leading zeros
  * [#10488](https://github.com/metasfresh/metasfresh/pull/10488) Rearrange procurement-WebUI folders
  * [#10493](https://github.com/metasfresh/metasfresh/issues/10493) Create `C_Title` and `C_Title_Trl`
  * [#10500](https://github.com/metasfresh/metasfresh/issues/10500) Create report for intratrade and intracommunity
  * [#10501](https://github.com/metasfresh/metasfresh/issues/10501) Extended Payment REST Endpoint
  * [#10515](https://github.com/metasfresh/metasfresh/issues/10515) Create `C_BPartner_Location.Setup_Place_No` field
  * [#10521](https://github.com/metasfresh/metasfresh/issues/10521) Add `isSupervisor` Column into `AD_User` table
  * [#10524](https://github.com/metasfresh/metasfresh/issues/10524) Customize Auftragsdisposition (Sales Order Candidates) Window
  * [#10526](https://github.com/metasfresh/metasfresh/issues/10526) Tabs and sections need to be configurable for export via data-entry-rest-controller
  * [#10531](https://github.com/metasfresh/metasfresh/issues/10531) Date 'Invoice from' as default filter date
  * [#10535](https://github.com/metasfresh/metasfresh/issues/10535) Additional String Accounting Dimensions
  * [#10536](https://github.com/metasfresh/metasfresh/issues/10536) Prevent multiple invoice reversals
  * [#10538](https://github.com/metasfresh/metasfresh/issues/10538) Move Haddex from Product to Partner
  * [#10540](https://github.com/metasfresh/metasfresh/issues/10540) Changes to `C_Invoice_Rejection_Detail` now published to `C_Invoice`
  * [#10555](https://github.com/metasfresh/metasfresh/issues/10555) Add Mass Print PDF process to Outbound Documents
  * [#10556](https://github.com/metasfresh/metasfresh/issues/10556) Remove unused `C_Payment_CreateFrom_BankStatement` process and references
  * [#10560](https://github.com/metasfresh/metasfresh/issues/10560) Prevent reverting inventories if HU was already transformed
  * [#10566](https://github.com/metasfresh/metasfresh/issues/10566) Add Document Sub Type = Requisition
  * [#10569](https://github.com/metasfresh/metasfresh/pull/10569) Picking v2 layout improvements
  * [#10570](https://github.com/metasfresh/metasfresh/pull/10570) Change remaining modules from jaxb2-maven-plugin to maven-jaxb2-plugin
  * [#10573](https://github.com/metasfresh/metasfresh/issues/10573) Increase Product eff. size, decrease Replication Transaction size
  * [#10575](https://github.com/metasfresh/metasfresh/issues/10575) Lookup anstatt Dropdown bei Bestellungen aus Auftrag generieren
  * [#10581](https://github.com/metasfresh/metasfresh/issues/10581) Filter für Gebinde in Rechnungsdispo ist nicht korrekt
  * [#10582](https://github.com/metasfresh/metasfresh/issues/10582) Allow user to choose if shall print logo or not when printing documents
  * [#10590](https://github.com/metasfresh/metasfresh/issues/10590) Extend BPartner-Relation and add it as BPartner-Tab
  * [#10594](https://github.com/metasfresh/metasfresh/issues/10594) Create `ExternalSystem_Config` Table and Window
  * [#10595](https://github.com/metasfresh/metasfresh/issues/10595) Remittance advice document
  * [#10607](https://github.com/metasfresh/metasfresh/issues/10607) Create REST Endpoint for external reference lookups and insertions
  * [#10617](https://github.com/metasfresh/metasfresh/pull/10617) Improve RestResponseEntityExceptionHandler's "default" method
  * [#10618](https://github.com/metasfresh/metasfresh/issues/10618) Add endpoint for `C_BP_Relation`
  * [#10619](https://github.com/metasfresh/metasfresh/pull/10619) WebUI json document field precision
  * [#10624](https://github.com/metasfresh/metasfresh/issues/10624) Print Selection of Doc Outbound logs
  * [#10634](https://github.com/metasfresh/metasfresh/pull/10634) `C_Payment.CurrencyRate` (intensive_care_hotfix)
  * [#10642](https://github.com/metasfresh/metasfresh/issues/10642) `DD_Order.Processed` - add a default falue
  * [#10644](https://github.com/metasfresh/metasfresh/issues/10644) Manufacturing REST API: Search HUs to Issue by HUValue and SerialNo
  * [#10676](https://github.com/metasfresh/metasfresh/issues/10676) Alberta Patients Import
  * [#10683](https://github.com/metasfresh/metasfresh/issues/10683) `AD_Issue` - Insert REST Endpoint

## Fixes
* metasfresh
  * [#10149](https://github.com/metasfresh/metasfresh/issues/10149) `/quickactions` endpoint is called twice first time with wrong params
  * [#10422](https://github.com/metasfresh/metasfresh/issues/10422) `MD_Stock.qtyOnHand` is not updated when completing inventory
  * [#10434](https://github.com/metasfresh/metasfresh/issues/10434) Creating bpartner on-the-fly not working correctly
  * [#10436](https://github.com/metasfresh/metasfresh/issues/10436) Jenkins: when running frontend tests use a random port
  * [#10450](https://github.com/metasfresh/metasfresh/issues/10450) Show more entries under navigation bookmark menu
  * [#10457](https://github.com/metasfresh/metasfresh/issues/10457) Prevent weird errors on login
  * [#10459](https://github.com/metasfresh/metasfresh/issues/10459) Dropdown appears, but it is not possible to add something from it when you click
  * [#10469](https://github.com/metasfresh/metasfresh/issues/10469) Investigate failing tests that might be introduced in period Nov-Dec
  * [#10471](https://github.com/metasfresh/metasfresh/issues/10471) Performance window accounting transactions on erpwebui
  * [#10474](https://github.com/metasfresh/metasfresh/issues/10474) Price override on empty cells
  * [#10483](https://github.com/metasfresh/metasfresh/issues/10483) Always set `C_Invoice_candidate.IsEDIEnabled` to `N` if bpartner is no invoice recipient
  * [#10490](https://github.com/metasfresh/metasfresh/issues/10490) Fix M_Locator-Indices
  * [#10491](https://github.com/metasfresh/metasfresh/issues/10491) Received CUs serial number correction
  * [#10497](https://github.com/metasfresh/metasfresh/issues/10497) `I_BankStatement.DebitOrCreditIndicator` interchange
  * [#10503](https://github.com/metasfresh/metasfresh/issues/10503) Allocation Tab sometimes missing in vendor invoice window
  * [#10507](https://github.com/metasfresh/metasfresh/issues/10507) Lagerwert (Excel): convert cost price into the UOM displayed in the report line
  * [#10513](https://github.com/metasfresh/metasfresh/issues/10513) Lagerwert (Excel): the product and warehouse parameters are not respected
  * [#10529](https://github.com/metasfresh/metasfresh/issues/10529) Lagerwert (Excel): rounding for the amount
  * [#10547](https://github.com/metasfresh/metasfresh/issues/10547) Creating rows in subtab of Bank Statement via import not working
  * [#10578](https://github.com/metasfresh/metasfresh/issues/10578) Issue from multiple HUs
  * [#10580](https://github.com/metasfresh/metasfresh/issues/10580) Avoid NPE when loading order line candidate via replication interface
  * [#10589](https://github.com/metasfresh/metasfresh/issues/10589) Order reference not copied from quotation process parameter
  * [#10591](https://github.com/metasfresh/metasfresh/issues/10591) CU label not available anymore in manufacturing order
  * [#10598](https://github.com/metasfresh/metasfresh/pull/10598) Add a fix to display the view `C_Printing_Queue_PrintInfo_v` in WebUI
  * [#10599](https://github.com/metasfresh/metasfresh/issues/10599) Payment allocation accounting: correction
  * [#10609](https://github.com/metasfresh/metasfresh/issues/10609) FE Shortcut does not work in the modal for selecting print logo Y/N
  * [#10614](https://github.com/metasfresh/metasfresh/issues/10614) Valid combination not created after new element
  * [#10630](https://github.com/metasfresh/metasfresh/issues/10630) Investigate failing tests that might be introduced in period Ian- beginning of Feb 2021
  * [#10635](https://github.com/metasfresh/metasfresh/pull/10635) Payment allocation: use max date between invoice and payment
  * [#10649](https://github.com/metasfresh/metasfresh/issues/10649) Document actions element doesn't hide
  * [#10652](https://github.com/metasfresh/metasfresh/issues/10652) Incorrect breadcrumb after logout & login
  * [#10656](https://github.com/metasfresh/metasfresh/issues/10656) Inventory import w/o HU aggregation type: Use multiple as default

# metasfresh 5.160
## Features
* metasfresh
  * [#10035](https://github.com/metasfresh/metasfresh/issues/10035) Can't sort by ID type virtual columns in grid view
  * [#10184](https://github.com/metasfresh/metasfresh/issues/10184) WebUI: Implement User approval workflows
  * [#10187](https://github.com/metasfresh/metasfresh/issues/10187) Extend shipment-candidate exported infos
  * [#10191](https://github.com/metasfresh/metasfresh/issues/10191) UX: Error Messages
  * [#10192](https://github.com/metasfresh/metasfresh/issues/10192) Some custom queries aren't working
  * [#10203](https://github.com/metasfresh/metasfresh/pull/10203) Create Sales Order from this Quotation: don't show the action if it does not apply
  * [#10206](https://github.com/metasfresh/metasfresh/issues/10206) Async/bounce cache invalidation and websocket events
  * [#10208](https://github.com/metasfresh/metasfresh/pull/10208) Avoid using Postgres OID
  * [#10210](https://github.com/metasfresh/metasfresh/issues/10210) Disable DocAction button while processing
  * [#10221](https://github.com/metasfresh/metasfresh/issues/10221) Allow movements from source HUs
  * [#10226](https://github.com/metasfresh/metasfresh/issues/10226) Add Validation Rule to display only the last 3 newest price list versions
  * [#10231](https://github.com/metasfresh/metasfresh/issues/10231) Add Packaging-GTINs to Desadv-Pack
  * [#10232](https://github.com/metasfresh/metasfresh/issues/10232) Update `AD_Process.Name` when editing `AD_Process_Trl.Name` for base language
  * [#10238](https://github.com/metasfresh/metasfresh/issues/10238) Add SQL For Current vs Next price list comparison
  * [#10242](https://github.com/metasfresh/metasfresh/issues/10242) Report - Quotation: handle `PRINTER_OPTS_IsPrintLogo`, `PRINTER_OPTS_IsPrintTotals` parameters
  * [#10244](https://github.com/metasfresh/metasfresh/pull/10244) More info if ESR-check-digit computation fails for SEPA_Export_Line
  * [#10245](https://github.com/metasfresh/metasfresh/issues/10245) Display Discontinued Flag for product and add Process to activate ProductPrice based on the flag
  * [#10246](https://github.com/metasfresh/metasfresh/pull/10246) Printing Options
  * [#10252](https://github.com/metasfresh/metasfresh/issues/10252) Mark Country ID as mandatory in the area search filters
  * [#10262](https://github.com/metasfresh/metasfresh/issues/10262) Cypress test for UI Element Labels
  * [#10264](https://github.com/metasfresh/metasfresh/issues/10264) Support for using the login user as default filter
  * [#10266](https://github.com/metasfresh/metasfresh/issues/10266) Activate changelog
  * [#10267](https://github.com/metasfresh/metasfresh/issues/10267) Add Movement Type Filter to Product Transactions window
  * [#10270](https://github.com/metasfresh/metasfresh/issues/10270) Bank Statement Import improvements
  * [#10273](https://github.com/metasfresh/metasfresh/pull/10273) `C_Invoice_Candidate_Recompute`: add PK
  * [#10279](https://github.com/metasfresh/metasfresh/issues/10279) Add Marketing Channel Attribute and Window to User
  * [#10283](https://github.com/metasfresh/metasfresh/pull/10283) Make sure that we specify if date-without-time shall be 00:00 or 23:59
  * [#10291](https://github.com/metasfresh/metasfresh/issues/10291) Warehouse in Picking Terminal v2 Filter
  * [#10293](https://github.com/metasfresh/metasfresh/issues/10293) Router Attributes
  * [#10298](https://github.com/metasfresh/metasfresh/pull/10298) Redistribute syncadvise when creating bpartner from olcand-bpartner info
  * [#10302](https://github.com/metasfresh/metasfresh/issues/10302) Manufacturing extensions
  * [#10304](https://github.com/metasfresh/metasfresh/issues/10304) Put toast notification in place with close icon
  * [#10310](https://github.com/metasfresh/metasfresh/issues/10310) Manufacturing extension: material dispo shall work with `PP_Product_Planning.MaxManufacturedQtyPerOrder`
  * [#10312](https://github.com/metasfresh/metasfresh/pull/10312) Remove popup about missing app server when starting swing
  * [#10316](https://github.com/metasfresh/metasfresh/issues/10316) Adding a LeadTime column and display on the Product Business Partner Tab
  * [#10318](https://github.com/metasfresh/metasfresh/issues/10318) Reuse last archive if no info available when creating reports
  * [#10321](https://github.com/metasfresh/metasfresh/issues/10321) Add new font icons
  * [#10323](https://github.com/metasfresh/metasfresh/issues/10323) Add flag to disable marketing contact creation
  * [#10325](https://github.com/metasfresh/metasfresh/issues/10325) Print manufacturing order label
  * [#10327](https://github.com/metasfresh/metasfresh/issues/10327) Material schedule improvements
  * [#10332](https://github.com/metasfresh/metasfresh/pull/10332) Improve `migrationscript_ignore` error handling
  * [#10336](https://github.com/metasfresh/metasfresh/issues/10336) Order printing options: only display totals when needed
  * [#10338](https://github.com/metasfresh/metasfresh/issues/10338) Add dedicated REST-Endpoint for municipality invoices
  * [#10340](https://github.com/metasfresh/metasfresh/issues/10340) Unlink Quotation/Order before deleting
  * [#10348](https://github.com/metasfresh/metasfresh/issues/10348) Create Scheduler for minus skonto
  * [#10357](https://github.com/metasfresh/metasfresh/issues/10357) Add `M_Warehouse_ID` to `C_OLCand`
  * [#10365](https://github.com/metasfresh/metasfresh/issues/10365) Always update `SalesOrderLine.Price*` when SalesOrder.DatePromissed is changed
  * [#10368](https://github.com/metasfresh/metasfresh/issues/10368) Do not show by-product on manufacturing order report
  * [#10371](https://github.com/metasfresh/metasfresh/issues/10371) Add new column to `r_request` table
  * [#10374](https://github.com/metasfresh/metasfresh/pull/10374) Customize Tabs for "Service Annahme" Window
  * [#10375](https://github.com/metasfresh/metasfresh/issues/10375) Introduce new `ad_messages`
  * [#10377](https://github.com/metasfresh/metasfresh/issues/10377) Service Orders: create Request from `M_InOut` if configured
  * [#10378](https://github.com/metasfresh/metasfresh/issues/10378) Product proposal: only allow prices in the same currency as the source order
  * [#10383](https://github.com/metasfresh/metasfresh/pull/10383) Changing reference to search in base price list
  * [#10409](https://github.com/metasfresh/metasfresh/issues/10409) Adding filter for creating new order from quotation
  * [#10414](https://github.com/metasfresh/metasfresh/issues/10414) Guarantee/Service: Own window for Service Handling Units
  * [#10415](https://github.com/metasfresh/metasfresh/issues/10415) Action to open the Service HU Editor from "Service Annahme" window
  * [#10417](https://github.com/metasfresh/metasfresh/pull/10417) When splitting the HU in `QtyCU`=1 HUs, make sure the `PP_Order_Qty.Qty` is also ONE
  * [#10433](https://github.com/metasfresh/metasfresh/pull/10433) Add property `skipIfIndirectlyCalled` to annotation `CalloutMethod`

* metasfresh-webui-frontend-legacy
  * [#2656](https://github.com/metasfresh/metasfresh-webui-frontend-legacy/issues/2656) UX: Error Messages

## Fixes
* metasfresh
  * [#9867](https://github.com/metasfresh/metasfresh/pull/9867) OLCand-API's BPartner lookup ignores Org
  * [#10196](https://github.com/metasfresh/metasfresh/pull/10196) Fix NPE on missing currency conversion
  * [#10197](https://github.com/metasfresh/metasfresh/issues/10197) Sales Order window: avoid setting a DocType if is not in the list that user can pick from
  * [#10201](https://github.com/metasfresh/metasfresh/issues/10201) Error when setting attributes in orderline
  * [#10204](https://github.com/metasfresh/metasfresh/issues/10204) Label UI Elements: respect reference and valrule from `AD_Field`
  * [#10211](https://github.com/metasfresh/metasfresh/issues/10211) Browser back button does not work correctly when starting tab using a direct link
  * [#10224](https://github.com/metasfresh/metasfresh/pull/10224) Replication - boolean fields need to export `Y` or `N`, not `true` or `false`
  * [#10228](https://github.com/metasfresh/metasfresh/issues/10228) Request.EndDate gets reset when setting another field
  * [#10230](https://github.com/metasfresh/metasfresh/issues/10230) Advanced Edit - View jumping to end of list
  * [#10247](https://github.com/metasfresh/metasfresh/pull/10247) On any RuntimeException flag shipmentCandidate as "error" and move on
  * [#10254](https://github.com/metasfresh/metasfresh/issues/10254) Fix Manufacturing Order printing
  * [#10276](https://github.com/metasfresh/metasfresh/issues/10276) Some windows not usable sometimes in case of mass shipping / mass invoicing
  * [#10278](https://github.com/metasfresh/metasfresh/pull/10278) Prevent multiple re-renderings
  * [#10287](https://github.com/metasfresh/metasfresh/issues/10287) Invoice is not ispaid = Y although fully allocated
  * [#10307](https://github.com/metasfresh/metasfresh/issues/10307) Packing instructions available in sales order batch entry although not on price list
  * [#10330](https://github.com/metasfresh/metasfresh/issues/10330) Fix for partner lookup when imported from OLCand
  * [#10347](https://github.com/metasfresh/metasfresh/pull/10347) Also filter by product when resolving HUs
  * [#10352](https://github.com/metasfresh/metasfresh/pull/10352) Add `outputDirectory` configuration to jaxb2
  * [#10354](https://github.com/metasfresh/metasfresh/pull/10354) Hotfix WebUI convert from boolean to string lookup value
  * [#10385](https://github.com/metasfresh/metasfresh/pull/10385) Hotfix `DataTypes.convertToBigDecimal`: handle Quantity too
  * [#10396](https://github.com/metasfresh/metasfresh/issues/10396) REST Endpoint for Invoice data Query by customer
  * [#10397](https://github.com/metasfresh/metasfresh/issues/10397) Reference to commission Invoice candidate is missing in commission deed
  * [#10406](https://github.com/metasfresh/metasfresh/pull/10406) Error attaching Sales Order to Customer Return window

# metasfresh 5.159
## Features
* metasfresh
  * [#10023](https://github.com/metasfresh/metasfresh/issues/10023) Payment service providers also calculate fee on credit memos
  * [#10174](https://github.com/metasfresh/metasfresh/issues/10174) Unskip modal tests
  * [#10175](https://github.com/metasfresh/metasfresh/issues/10175) Avoid timeouts while cleaning up old `T_Query_Selection_*` records

## Fixes
* metasfresh
  * [#10078](https://github.com/metasfresh/metasfresh/issues/10078) Wrong costs for manufacturing finished goods

# metasfresh 5.158
## Features
* metasfresh
  * [#9944](https://github.com/metasfresh/metasfresh/issues/9944) Include product commodity number in the receipt schedule export REST endpoint
  * [#10094](https://github.com/metasfresh/metasfresh/issues/10094) Create shipping packages REST endpoint
  * [#10127](https://github.com/metasfresh/metasfresh/issues/10127) Transfer complete sales order in \_bestell-XML
  * [#10130](https://github.com/metasfresh/metasfresh/issues/10130) QR Code disabled by default
  * [#10143](https://github.com/metasfresh/metasfresh/issues/10143) Status changes for DESADV
  * [#10150](https://github.com/metasfresh/metasfresh/issues/10150) Avoid concurrent shipment-creation and shipment-schedule updating
  * [#10167](https://github.com/metasfresh/metasfresh/issues/10167) Allow deselecting rows when mouse clicking

## Fixes
* metasfresh
  * [#10157](https://github.com/metasfresh/metasfresh/issues/10157) Bug on order counter document creation: DocTypeTarget set for initial order, not for counter
  * [#10159](https://github.com/metasfresh/metasfresh/issues/10159) Picking list issue - double entries in some cases
  * [#10161](https://github.com/metasfresh/metasfresh/issues/10161) Bug when creating business partner *and group* on the fly
  * [#10165](https://github.com/metasfresh/metasfresh/issues/10165) Payment allocation: outbound payment, vendor invoice, vendor CM not working

# metasfresh 5.157
## Features
* metasfresh
  * [#10106](https://github.com/metasfresh/metasfresh/issues/10106) Add Raw Material Origin and NetWeight into Product

## Fixes
* metasfresh
  * [#10132](https://github.com/metasfresh/metasfresh/issues/10132) Fix never ending migration script 5569290_sys_gh10046_setPoReferenceToShipmentSchedule
  * [#10135](https://github.com/metasfresh/metasfresh/issues/10135) WebUI Front End: Removing labels is annoying and not smooth
  * [#10139](https://github.com/metasfresh/metasfresh/issues/10139) "Add new" button not displayed after adding a new entry was unsuccessful/aborted
  * [#10142](https://github.com/metasfresh/metasfresh/issues/10142) Labels component is not respecting read-only property
  * [#10145](https://github.com/metasfresh/metasfresh/issues/10145) Phone Call Schedule: After action 'create sales order' was called, the action is not available anymore

# metasfresh 5.156
## Features
* metasfresh
  * [#9886](https://github.com/metasfresh/metasfresh/issues/9886) Filter: Invoice disposition by "reference" = delivery note number entered in the order
  * [#9938](https://github.com/metasfresh/metasfresh/issues/9938) Display the field AD_Tab in the Table-Process tab of the Process window (WebUI)
  * [#9958](https://github.com/metasfresh/metasfresh/issues/9958) Fix ProductPlanning creation and Org
  * [#9966](https://github.com/metasfresh/metasfresh/issues/9966) Add support for CSV-Response in postgREST-Processes
  * [#10001](https://github.com/metasfresh/metasfresh/issues/10001) Add M_Warehouse in C_Invoice and use it for tax calculation
  * [#10022](https://github.com/metasfresh/metasfresh/issues/10022) Automatically set `HU.BestBeforeDate` and `HU.LotNr` attributes during Manfacturing
  * [#10034](https://github.com/metasfresh/metasfresh/issues/10034) Add possibility to open documents created from processes in new tabs
  * [#10059](https://github.com/metasfresh/metasfresh/issues/10059) Invoice and Order: Only allow doctypes with the same org as the document or *
  * [#10074](https://github.com/metasfresh/metasfresh/issues/10074) Create metasfresh window for 'Purchase Invoice Candidates'
  * [#10076](https://github.com/metasfresh/metasfresh/issues/10076) Rename parameter Label at "Gutschrift erstellen"
  * [#10079](https://github.com/metasfresh/metasfresh/issues/10079) Add window 'Counter Document' and 'Missing/Incomplete Counter Document' to WebUI role
  * [#10083](https://github.com/metasfresh/metasfresh/issues/10083) Make it easier to work with API export status from metasfresh
  * [#10088](https://github.com/metasfresh/metasfresh/issues/10088) Filter out closed shipment schedules from picking terminal window
  * [#10097](https://github.com/metasfresh/metasfresh/issues/10097) Include sequence number in exports for shipment-candidate, receipt-candidate and production-order
  * [#10098](https://github.com/metasfresh/metasfresh/issues/10098) Assign Material receipt to the project
  * [#10108](https://github.com/metasfresh/metasfresh/issues/10108) Introduce AD_UI_Section.UIStyle
  * [#10114](https://github.com/metasfresh/metasfresh/pull/10114) Add special auto-vacuum settings for different tables
  * [#10122](https://github.com/metasfresh/metasfresh/issues/10122) Picking Tray Cleaning: add QtyTU parameter to "Take out and add to LU" process

## Fixes
* metasfresh
  * [#10045](https://github.com/metasfresh/metasfresh/issues/10045) Packing instructions are no longer displayed when ordering
  * [#10068](https://github.com/metasfresh/metasfresh/issues/10068) Reactivate sales order fix
  * [#10084](https://github.com/metasfresh/metasfresh/issues/10084) DatePromised and PreparationDate shall be copied From Offer when creating a sales order
  * [#10116](https://github.com/metasfresh/metasfresh/issues/10116) Created two entries through double click
  * [#10121](https://github.com/metasfresh/metasfresh/pull/10121) Update lombok to 1.18.14 from 1.18.10
  * [#10125](https://github.com/metasfresh/metasfresh/issues/10125) Fix editing fields in data entry tabs

# metasfresh 5.155
## Features
* metasfresh
  * [#9914](https://github.com/metasfresh/metasfresh/issues/9914) Create a data wrapper for the widgets
  * [#9931](https://github.com/metasfresh/metasfresh/issues/9931) XML <-> metasfresh inventory import
  * [#9976](https://github.com/metasfresh/metasfresh/issues/9976) Add number of exported shipment schedule items to REST-API
  * [#10003](https://github.com/metasfresh/metasfresh/issues/10003) Increase `AD_Process.JsonPath` column size
  * [#10009](https://github.com/metasfresh/metasfresh/issues/10009) Out-of-stock correction via camel
  * [#10010](https://github.com/metasfresh/metasfresh/issues/10010) Reference between organisation master data and business partner
  * [#10015](https://github.com/metasfresh/metasfresh/pull/10015) Manufacturing issue/receipt import audit
  * [#10017](https://github.com/metasfresh/metasfresh/issues/10017) Export `Order.deliveryInfo` via camel
  * [#10020](https://github.com/metasfresh/metasfresh/pull/10020) Camel: write error file
  * [#10027](https://github.com/metasfresh/metasfresh/issues/10027) Drop column `R_Request.StartDate`
  * [#10038](https://github.com/metasfresh/metasfresh/issues/10038) Open newly created documents in a new tab
  * [#10046](https://github.com/metasfresh/metasfresh/issues/10046) Change columnsql of `FilteredItemsWithSameHeaderAggregationKey` column
  * [#10050](https://github.com/metasfresh/metasfresh/pull/10050) Replace `Purchase Order` tab `OrderByClause` with `AD_Field.SortNo`
  * [#10057](https://github.com/metasfresh/metasfresh/issues/10057) Service provider platform enhancements

## Fixes
* metasfresh
  * [#10030](https://github.com/metasfresh/metasfresh/issues/10030) Do not add duplicate filters to a view
  * [#10037](https://github.com/metasfresh/metasfresh/pull/10037) HU matching fixes
  * [#10041](https://github.com/metasfresh/metasfresh/issues/10041) Don't crash the app when widget exists in layout but not data
  * [#10051](https://github.com/metasfresh/metasfresh/issues/10051) Invoice DocType is taken from login Org instead of the invoice candidates' one

# metasfresh 5.154
## Features
* metasfresh
  * [#9971](https://github.com/metasfresh/metasfresh/issues/9971) Allow 'Issue'ing of 'By-Product' and 'Co-Product' created HUs in manufacturing
  * [#9982](https://github.com/metasfresh/metasfresh/issues/9982) Create shipments REST-API adjustments
  * [#9984](https://github.com/metasfresh/metasfresh/pull/9984) Store the data in the redux store instead of local state

## Fixes
* metasfresh
  * [#9975](https://github.com/metasfresh/metasfresh/issues/9975) Browser Back stops at Dashboard
  * [#9980](https://github.com/metasfresh/metasfresh/issues/9980) Order indicator vanished after switching detail view back to grid view
  * [#9988](https://github.com/metasfresh/metasfresh/issues/9988) Avoid duplicate records in AD_TreeBar
  * [#9993](https://github.com/metasfresh/metasfresh/issues/9993) Use a nonce in Convert methods
  * [#9999](https://github.com/metasfresh/metasfresh/issues/9999) Documents cannot be voided
  * [#10000](https://github.com/metasfresh/metasfresh/pull/10000) Add missing prompt from the state
  * [#10005](https://github.com/metasfresh/metasfresh/issues/10005) Allocating entries in Allocate Payments overlay only works once
  * [#10007](https://github.com/metasfresh/metasfresh/pull/10007) Fixes for Dashboard breadcrumbs path

# metasfresh 5.153
## Features
* metasfresh
  * [#9877](https://github.com/metasfresh/metasfresh/issues/9877) Manufacturing REST API
  * [#9920](https://github.com/metasfresh/metasfresh/issues/9920) Handle good returns via REST-API
  * [#9926](https://github.com/metasfresh/metasfresh/issues/9926) Enhance HU Transformation process to allow movement of the created HUs
  * [#9933](https://github.com/metasfresh/metasfresh/issues/9933) Receipt API enhancement
  * [#9935](https://github.com/metasfresh/metasfresh/issues/9935) Assign deliveries and invoices to the project, automatically and manually
  * [#9946](https://github.com/metasfresh/metasfresh/issues/9946) Cancel Date filter
  * [#9948](https://github.com/metasfresh/metasfresh/issues/9948) Insert UOM in 'Produkt Transaktionen' window
  * [#9951](https://github.com/metasfresh/metasfresh/issues/9951) Add Croatia to country area table for EU
  * [#9954](https://github.com/metasfresh/metasfresh/issues/9954) Adjustments for export shipment schedules API
  * [#9969](https://github.com/metasfresh/metasfresh/issues/9969) Order from quotation (construction), reference to quotation

## Fixes
* metasfresh
  * [#9923](https://github.com/metasfresh/metasfresh/pull/9923) Fix swing's wrong language on machine
  * [#9930](https://github.com/metasfresh/metasfresh/pull/9930) Fix scroll in expanded mode
  * [#9940](https://github.com/metasfresh/metasfresh/issues/9940) Sales Order: Allow multiple decimals
  * [#9942](https://github.com/metasfresh/metasfresh/pull/9942) Fix qty input batch entry
  * [#9943](https://github.com/metasfresh/metasfresh/pull/9943) Fix `de.metas.printing.common` pom
  * [#9947](https://github.com/metasfresh/metasfresh/issues/9947) Zoom into links in subtabs sometimes cut off

# metasfresh 5.152
## Features
* metasfresh
  * [#9877](https://github.com/metasfresh/metasfresh/issues/9877) Manufacturing REST API
  * [#9895](https://github.com/metasfresh/metasfresh/issues/9895) Implement display logic for Labels
  * [#9897](https://github.com/metasfresh/metasfresh/issues/9897) Support Payment Allocation with different currencies
  * [#9901](https://github.com/metasfresh/metasfresh/issues/9901) Extend REST API for Invoice Detail Item
  * [#9908](https://github.com/metasfresh/metasfresh/issues/9908) Simplify approval in order planning

## Fixes
* metasfresh
  * [#9916](https://github.com/metasfresh/metasfresh/issues/9916) White grid after browser back button in "Anrufliste"
  * [#9919](https://github.com/metasfresh/metasfresh/issues/9919) Throw an error when there is no Transit Locator when completing a DD Order
  * [#9898](https://github.com/metasfresh/metasfresh/issues/9898) Zoom into product prices from PLV not working

# metasfresh 5.151
## Features
* metasfresh
  * [#7175](https://github.com/metasfresh/metasfresh/pull/7175) Improve usability of PostgREST export processes
  * [#9838](https://github.com/metasfresh/metasfresh/issues/9838) Add SeqNo on AD_language
  * [#9855](https://github.com/metasfresh/metasfresh/issues/9855) Inventory - Automatically destroy HUs with stock 0
  * [#9860](https://github.com/metasfresh/metasfresh/issues/9860) BOM verified in product window show main grid + filter
  * [#9862](https://github.com/metasfresh/metasfresh/issues/9862) Show serial number in production HU selection window
  * [#9863](https://github.com/metasfresh/metasfresh/issues/9863) Allow creation of credit memo for invoices already flagged as paid
  * [#9868](https://github.com/metasfresh/metasfresh/issues/9868) Enhance upload receipt and shipment candidates URI flexibility
  * [#9878](https://github.com/metasfresh/metasfresh/issues/9878) Provide stock value as download according to specific date
  * [#9880](https://github.com/metasfresh/metasfresh/issues/9880) Customer returns window adjustment

## Fixes
* metasfresh
  * [#7073](https://github.com/metasfresh/metasfresh/issues/7073) GL Journal Lines with TAX Amount 0 can't be booked, many 🙏 to [Peter Wyss (@KommunikativCh)](https://github.com/KommunikativCh)
  * [#9871](https://github.com/metasfresh/metasfresh/issues/9871) Inactive contacts can't be set to active again
  * [#9873](https://github.com/metasfresh/metasfresh/issues/9873) Extend business partner import to care about Org

# metasfresh 5.150
## Features
* metasfresh
  * [#7137](https://github.com/metasfresh/metasfresh/pull/7137) Always capture previous costs
  * [#7140](https://github.com/metasfresh/metasfresh/issues/7140) Small changes for data Exchange with Logistics company
  * [#7142](https://github.com/metasfresh/metasfresh/issues/7142) OLCand/BPartner REST Endpoints: import C_BPartner.VATaxId
  * [#7159](https://github.com/metasfresh/metasfresh/issues/7159) Add prepayment check in sales order functions
  * [#7173](https://github.com/metasfresh/metasfresh/issues/7173) Add product weight in de_metas_endcustomer_fresh_reports.Docs_Sales_Order_Details
  * [#7182](https://github.com/metasfresh/metasfresh/pull/7182) Improve sales invoice status endpoint
  * [#7186](https://github.com/metasfresh/metasfresh/issues/7186) Receipt REST-Api: Create material receipts
  * [#7171](https://github.com/metasfresh/metasfresh/issues/7171) Order candidates processing: Paypal/ creditcard payments w/ reference and prepayment

## Fixes
* metasfresh
  * [#7073](https://github.com/metasfresh/metasfresh/issues/7073) Many 🙏 to [Peter Wyss (@KommunikativCh)](https://github.com/KommunikativCh)
  * [#7127](https://github.com/metasfresh/metasfresh/issues/7127) Problem: pressing esc after editing field shows typed value, instead of existing one (old one)
  * [#7158](https://github.com/metasfresh/metasfresh/issues/7158) Quick edit modal overlay not refreshed after attribute edit
  * [#7161](https://github.com/metasfresh/metasfresh/pull/7161) Fix NPE if an invoice candidate is in catch weight but none is given
  * [#7166](https://github.com/metasfresh/metasfresh/pull/7166) Rüstschein modal overlay not refreshed after attribute edit
  * [#7177](https://github.com/metasfresh/metasfresh/issues/7177) Dropdown behaves weird when two elements with the same key exist in the list
  * [#7183](https://github.com/metasfresh/metasfresh/issues/7183) Kontakte Mobil Start date not initially set
  * [#9839](https://github.com/metasfresh/metasfresh/pull/9839) Remove rabbitmq swing error
  * [#9840](https://github.com/metasfresh/metasfresh/issues/9840) Jenkins build is broken on the frontend part

# metasfresh 5.149
## Features
* metasfresh
  * [#3856](https://github.com/metasfresh/metasfresh/issues/3856) WebUI Forecast Window hide Calendar, Period, Year
  * [#7124](https://github.com/metasfresh/metasfresh/pull/7124) Product Price Table editing, shortcut, marked text
  * [#7142](https://github.com/metasfresh/metasfresh/issues/7142) OLCand/BPartner REST Endpoints: import C_BPartner.VATaxId
  * [#7148](https://github.com/metasfresh/metasfresh/issues/7148) Produktionsbericht: Produkt Name
  * [#7152](https://github.com/metasfresh/metasfresh/issues/7152) Flickering window after starting process on other machine
  * [#7155](https://github.com/metasfresh/metasfresh/issues/7155) Window layout improvements: current costs

## Fixes
* metasfresh
  * [#7083](https://github.com/metasfresh/metasfresh/issues/7083) When filtering and hiding/showing modals the redux state is not cleaned
  * [#7105](https://github.com/metasfresh/metasfresh/issues/7105) Window goes blank when reloaded after clicking the navigation link
  * [#9847](https://github.com/metasfresh/metasfresh/issues/9847) CU Label not working Error: Cannot convert HUReport_541195

# metasfresh 5.148
## Features
* metasfresh
  * [#6867](https://github.com/metasfresh/metasfresh/issues/6867) Import Cost Prices with 0 qty
  * [#7036](https://github.com/metasfresh/metasfresh/issues/7036) Add more unit tests
  * [#7085](https://github.com/metasfresh/metasfresh/issues/7085) Extend DESADV for DELV vs ULCO
  * [#7106](https://github.com/metasfresh/metasfresh/issues/7106) Allow "Verdichtung" (consolidation) on a whole Picking Slot (not just TU)
  * [#7117](https://github.com/metasfresh/metasfresh/issues/7117) Budget Issue tracking enhancements

## Fixes
* metasfresh
  * [#7128](https://github.com/metasfresh/metasfresh/issues/7128) Modal overlay for creating bpartner on-the-fly does not close

# metasfresh 5.147
## Features
* metasfresh
  * [#6714](https://github.com/metasfresh/metasfresh/issues/6714) ESR_Import: introduce IsReconciled flag same as we have in PaySelection
  * [#7036](https://github.com/metasfresh/metasfresh/issues/7036) Add more unit tests
  * [#7058](https://github.com/metasfresh/metasfresh/issues/7058) Automatic DD Order Movement
  * [#7064](https://github.com/metasfresh/metasfresh/issues/7064) Create a new structure for Allergen traces in the product as a new tab
  * [#7089](https://github.com/metasfresh/metasfresh/issues/7089) Show in Main and Grid view that a Notice/Comment is available
  * [#7093](https://github.com/metasfresh/metasfresh/issues/7093) New Column in contract that always shows the sales order that initiated the contract
  * [#7101](https://github.com/metasfresh/metasfresh/issues/7101) Picking Terminal improvements

## Fixes
* metasfresh
  * [#7097](https://github.com/metasfresh/metasfresh/issues/7097) Bank Statement not imported until the end

# metasfresh 5.146
## Features
* metasfresh
  * [#5493](https://github.com/metasfresh/metasfresh/issues/5493) Allow copy for M_Pricelist_Version
  * [#7015](https://github.com/metasfresh/metasfresh/issues/7015) Exclude OnCredit from DirectDebit MatchRequirement
  * [#7075](https://github.com/metasfresh/metasfresh/issues/7075) Force pick to existing HU

## Fixes
* metasfresh
  * [#6420](https://github.com/metasfresh/metasfresh/issues/6420) Customer return not working bc HUs cannot be selected
  * [#6526](https://github.com/metasfresh/metasfresh/issues/6526) Export SEPA Pain_001_001_03_CH_02 wrong xsi:schemaLocation 🙏 to [Peter Wyss (@KommunikativCh)](https://github.com/KommunikativCh)
  * [#6967](https://github.com/metasfresh/metasfresh/issues/6967) Refreshing page looses pagination 🙏 to [Merry Space (@PureLandFlying)](https://github.com/PureLandFlying)
  * [#7029](https://github.com/metasfresh/metasfresh/issues/7029) QR Code Implementation de_metas_endcustomer_fresh_reports.docs_sales_invoice_qr_code 🙏 to [Peter Wyss (@KommunikativCh)](https://github.com/KommunikativCh)
  * [#7044](https://github.com/metasfresh/metasfresh/issues/7044) Fix Corner Case for Reference from Product to BOM Component
  * [#7046](https://github.com/metasfresh/metasfresh/pull/7046) Fix regarding sync-advise "IfExists.DONT_UPDATE"
  * [#7069](https://github.com/metasfresh/metasfresh/issues/7069) Product allergen tab is not linked properly to Product

# metasfresh 5.145
## Features
* metasfresh
  * [#5484](https://github.com/metasfresh/metasfresh/issues/5484) Seminar / Training Course Management based on Projects
  * [#5816](https://github.com/metasfresh/metasfresh/issues/5816) Effort based invoicing for service companies
  * [#6205](https://github.com/metasfresh/metasfresh/issues/6205) Merge metasfresh-webui-api and metasfresh-dist into metasfresh
  * [#6285](https://github.com/metasfresh/metasfresh/issues/6285) Create a separate project for standalone material-dispo, printing, reporting services
  * [#6394](https://github.com/metasfresh/metasfresh/issues/6394) (Sales) Pricelist comparison new-last before new from menu for all Partners
  * [#6426](https://github.com/metasfresh/metasfresh/issues/6426) Fix 'Payment' window trls
  * [#6437](https://github.com/metasfresh/metasfresh/issues/6437) Campaign Price Window adjustment
  * [#6446](https://github.com/metasfresh/metasfresh/issues/6446) Show Own Palette in HU Editor
  * [#6451](https://github.com/metasfresh/metasfresh/issues/6451) Tax Report adjustments
  * [#6466](https://github.com/metasfresh/metasfresh/issues/6466) Material Receipt Candidates: Adjustments
  * [#6473](https://github.com/metasfresh/metasfresh/issues/6473) Tour version adjustments
  * [#6475](https://github.com/metasfresh/metasfresh/issues/6475) Pricelist export (Jasper & Excel) without HU_PI that are not on PL
  * [#6484](https://github.com/metasfresh/metasfresh/pull/6484) CompositeInterfaceWrapperHelper: getTrxName can throw exception
  * [#6485](https://github.com/metasfresh/metasfresh/issues/6485) PLV Name adjustment
  * [#6495](https://github.com/metasfresh/metasfresh/issues/6495) Case of NPE on reposting an invoice
  * [#6504](https://github.com/metasfresh/metasfresh/issues/6504) Add Swing "Chat" Feature to WebUI using name 'Comments'
  * [#6514](https://github.com/metasfresh/metasfresh/issues/6514) Forbid reconciliation of one payment with multiple bank statements
  * [#6520](https://github.com/metasfresh/metasfresh/issues/6520) Shipmentschedule & Invoice candidate recompute action
  * [#6529](https://github.com/metasfresh/metasfresh/issues/6529) Allow Invoice with Credit memo allocation
  * [#6537](https://github.com/metasfresh/metasfresh/issues/6537) Payment allocation Feature extended: Service Fees with Tax
  * [#6548](https://github.com/metasfresh/metasfresh/issues/6548) Lookup Process parameters shall allow inactive records
  * [#6575](https://github.com/metasfresh/metasfresh/issues/6575) Add missing Translations and Filter
  * [#6583](https://github.com/metasfresh/metasfresh/issues/6583) Fix Marginal Costing Short Version
  * [#6594](https://github.com/metasfresh/metasfresh/issues/6594) Trim Spaces from Search criteria in WebUI
  * [#6596](https://github.com/metasfresh/metasfresh/issues/6596) Do not fail on inactive partner locations on invoicing
  * [#6619](https://github.com/metasfresh/metasfresh/issues/6619) Handle C_Location-AD_ChangeLog with ValueNew=NULL gracefully
  * [#6631](https://github.com/metasfresh/metasfresh/pull/6631) Blue moon event tracing
  * [#6632](https://github.com/metasfresh/metasfresh/issues/6632) Remove obsolete 'org.compiere.model.I_C_BankAccount'
  * [#6656](https://github.com/metasfresh/metasfresh/issues/6656) Jasper: Layout of Pricelist report/ Pricelist comparison report
  * [#6667](https://github.com/metasfresh/metasfresh/issues/6667) Trl: WebUI forgotPassword messages
  * [#6670](https://github.com/metasfresh/metasfresh/issues/6670) Create new structure for recording Commodity Numbers
  * [#6674](https://github.com/metasfresh/metasfresh/issues/6674) Picking Window (v1) allow processing on Picking Slot selection
  * [#6682](https://github.com/metasfresh/metasfresh/issues/6682) Accounting Transactions adjustments
  * [#6694](https://github.com/metasfresh/metasfresh/issues/6694) Add 'Picked' flag on Picking Terminal window
  * [#6705](https://github.com/metasfresh/metasfresh/issues/6705) Allow EDI-Orders import via Excel
  * [#6709](https://github.com/metasfresh/metasfresh/issues/6709) Picking from Material Receipt Candidates Window HU Editor
  * [#6713](https://github.com/metasfresh/metasfresh/issues/6713) Window Distribution Order enhancements
  * [#6738](https://github.com/metasfresh/metasfresh/issues/6738) New Action and reduced window for Request
  * [#6743](https://github.com/metasfresh/metasfresh/issues/6743) Round up when converting UOMs
  * [#6747](https://github.com/metasfresh/metasfresh/issues/6747) 'Payment Allocation' action shall open also when Payments not available
  * [#6769](https://github.com/metasfresh/metasfresh/issues/6769) WebUI: payment allocation - book Bank Fee Amount
  * [#6771](https://github.com/metasfresh/metasfresh/issues/6771) Allow weighing in Picking Terminal v1
  * [#6801](https://github.com/metasfresh/metasfresh/issues/6801) EDI - Allow getting excel-files from remote SFTP
  * [#6803](https://github.com/metasfresh/metasfresh/issues/6803) Generate deliverydays for selected tourversion
  * [#6812](https://github.com/metasfresh/metasfresh/issues/6812) Commission calculation without invoicing
  * [#6819](https://github.com/metasfresh/metasfresh/issues/6819) introduce PostingError_Issue_ID to all accountable documents
  * [#6821](https://github.com/metasfresh/metasfresh/pull/6821) Allow wholeTax-taxes also if the document has IsTaxIncluded=N
  * [#6826](https://github.com/metasfresh/metasfresh/pull/6826) set guarantor-name as company name to the guarantor-address
  * [#6827](https://github.com/metasfresh/metasfresh/issues/6827) Extend Invoice reversal API to return affected ICs
  * [#6833](https://github.com/metasfresh/metasfresh/issues/6833) QR Code Implementation for Postfinance
  * [#6846](https://github.com/metasfresh/metasfresh/issues/6846) New Filters in 'Product Planning' Window
  * [#6850](https://github.com/metasfresh/metasfresh/issues/6850) Keep a unique window for Resource
  * [#6851](https://github.com/metasfresh/metasfresh/issues/6851) Store printing queue items in folder structure
  * [#6853](https://github.com/metasfresh/metasfresh/issues/6853) Store healthcare-ch XML invoice details as C_Invoice_Details
  * [#6856](https://github.com/metasfresh/metasfresh/issues/6856) New window for 'AD_Boilerplate_Trl'
  * [#6860](https://github.com/metasfresh/metasfresh/issues/6860) rearrange grid view marketing platform
  * [#6867](https://github.com/metasfresh/metasfresh/issues/6867) Import Cost Prices with 0 qty
  * [#6886](https://github.com/metasfresh/metasfresh/issues/6886) PP_Order_BOMLine - automatically set PP_Order's PP_Order_BOM_ID and M_Warehouse_ID
  * [#6887](https://github.com/metasfresh/metasfresh/issues/6887) Allow create Contracts in draft (docStatus: drafted)
  * [#6894](https://github.com/metasfresh/metasfresh/issues/6894) Add a default value of 10 for PP_ProductPlanning seqNo
  * [#6898](https://github.com/metasfresh/metasfresh/issues/6898) Avoid using C_UOM_Conversion.DivideRate
  * [#6900](https://github.com/metasfresh/metasfresh/issues/6900) Allow force picking without existing HUs
  * [#6904](https://github.com/metasfresh/metasfresh/issues/6904) Servicefees per Provider Customer
  * [#6919](https://github.com/metasfresh/metasfresh/issues/6919) Excel-Sales-Order with CU-UOM and CU-per-TU multiplier
  * [#6923](https://github.com/metasfresh/metasfresh/issues/6923) Picking Terminal (V2) Changes
  * [#6931](https://github.com/metasfresh/metasfresh/pull/6931) Add devices widget in the Quantity type
  * [#6945](https://github.com/metasfresh/metasfresh/issues/6945) Improve Tour Updating in Order
  * [#6949](https://github.com/metasfresh/metasfresh/issues/6949) 'Picking Terminal V2': Add process for picking and packing in 1 step
  * [#6956](https://github.com/metasfresh/metasfresh/issues/6956) Implement possibility to easy switch from QR Bill to ESR
  * [#6957](https://github.com/metasfresh/metasfresh/issues/6957) Add PostgREST process type
  * [#6980](https://github.com/metasfresh/metasfresh/pull/6980) event bus optimizations
  * [#6983](https://github.com/metasfresh/metasfresh/issues/6983) R_Request.SalesRep_ID repair default value
  * [#6985](https://github.com/metasfresh/metasfresh/issues/6985) Excel-Sales-Order Qty in Stock-UOM instead of Price-UOM
  * [#6987](https://github.com/metasfresh/metasfresh/issues/6987) Automatically mark all received HUs carrying BOM components as 'Source HUs'
  * [#7003](https://github.com/metasfresh/metasfresh/issues/7003) Option: C_Invoice_OnlyAllow_BillToDefault_Contact
  * [#7009](https://github.com/metasfresh/metasfresh/issues/7009) Copy w/ details for Manufacuring Order
  * [#7011](https://github.com/metasfresh/metasfresh/issues/7011) Make Replication Transactions process parameter a search field
  * [#7021](https://github.com/metasfresh/metasfresh/issues/7021) Picking Terminal V2: Pick&Pack: Skip rows with qty 0

* metasfresh-webui-api-legacy
  * [#1253](https://github.com/metasfresh/metasfresh-webui-api-legacy/issues/1253) Clone Details

* metasfresh-e2e-legacy
  * [#387](https://github.com/metasfresh/metasfresh-e2e-legacy/issues/387) Upgrade Cypress and make sure picking integration tests are working fine

## Fixes
* metasfresh
  * [#6299](https://github.com/metasfresh/metasfresh/issues/6299) Commission invoice candidates created too early, directly after sales order
  * [#6411](https://github.com/metasfresh/metasfresh/issues/6411) Mark all 'ExternalID' columns as 'IsCalculated'
  * [#6413](https://github.com/metasfresh/metasfresh/issues/6413) Dashboard throws error
  * [#6421](https://github.com/metasfresh/metasfresh/issues/6421) Flatrate term for commission can sometimes not be created bc mandatory field disappears
  * [#6442](https://github.com/metasfresh/metasfresh/issues/6442) Fix "update commission data" if there is already data for one contract
  * [#6449](https://github.com/metasfresh/metasfresh/issues/6449) Link from Bank Statement to Payment Selection doesn't work
  * [#6456](https://github.com/metasfresh/metasfresh/issues/6456) Window "Request for Proposal (Ausschreibung)": DocumentNo automatic
  * [#6464](https://github.com/metasfresh/metasfresh/issues/6464) Wrong BillTo location and contact when Sales Order created from PhonecallSchedule
  * [#6471](https://github.com/metasfresh/metasfresh/issues/6471) Co-Product in BOM not working
  * [#6477](https://github.com/metasfresh/metasfresh/issues/6477) Bug: Excel processes won't open
  * [#6482](https://github.com/metasfresh/metasfresh/issues/6482) Cloning with keyboard shortcut works even if action is hidden from menu
  * [#6488](https://github.com/metasfresh/metasfresh/issues/6488) Wrong number of pages displayed in pdf
  * [#6505](https://github.com/metasfresh/metasfresh/issues/6505) Fix problems related to SEPA credit transfer
  * [#6511](https://github.com/metasfresh/metasfresh/issues/6511) Bank statement line reference not marked as processed
  * [#6547](https://github.com/metasfresh/metasfresh/issues/6547) Cash Journal: Doubled lines after complete and Payment link to wrong line/wrong cashbook
  * [#6566](https://github.com/metasfresh/metasfresh/issues/6566) Repair Customer Retention logic
  * [#6573](https://github.com/metasfresh/metasfresh/issues/6573) Default Sorting Ingredients in Tableview and Product export
  * [#6579](https://github.com/metasfresh/metasfresh/issues/6579) Sales order with Payment Rule PayPal and no contact: NPE
  * [#6588](https://github.com/metasfresh/metasfresh/issues/6588) Jenkins build does not always pickup changes
  * [#6603](https://github.com/metasfresh/metasfresh/issues/6603) Pricelist Version Description wrong
  * [#6610](https://github.com/metasfresh/metasfresh/issues/6610) Material Withdrawal cannot run because wrong locator is detected
  * [#6615](https://github.com/metasfresh/metasfresh/issues/6615) Credit Memo with wrong included Tax created from invoice
  * [#6647](https://github.com/metasfresh/metasfresh/issues/6647) Dropdown list is not called with proper link in case of labels
  * [#6654](https://github.com/metasfresh/metasfresh/issues/6654) Mark column 'IsReconciled' as 'IsCalculated'
  * [#6662](https://github.com/metasfresh/metasfresh/issues/6662) Prices don't update in order line after Product Proposal update
  * [#6687](https://github.com/metasfresh/metasfresh/issues/6687) Optimize Screen behavior for "Rüstliste erfassen" in shipment schedule
  * [#6692](https://github.com/metasfresh/metasfresh/issues/6692) Facets seem to break process preconditions
  * [#6712](https://github.com/metasfresh/metasfresh/issues/6712) Incorrect format date when switching from US to DE or CH
  * [#6718](https://github.com/metasfresh/metasfresh/issues/6718) Verify/Fix UOM conversions from/to material dispo
  * [#6745](https://github.com/metasfresh/metasfresh/issues/6745) Fix completing inventory with lines that have an HU already assigned flow
  * [#6764](https://github.com/metasfresh/metasfresh/issues/6764) Sorting gets lost when flipping through pages
  * [#6777](https://github.com/metasfresh/metasfresh/issues/6777) Fix refresh after running a process
  * [#6782](https://github.com/metasfresh/metasfresh/issues/6782) Wrong Organisation set to HUs when doing Inventory or Material Receipt
  * [#6799](https://github.com/metasfresh/metasfresh/pull/6799) Fix accidental inactivation of not-IBAN bank accounts
  * [#6807](https://github.com/metasfresh/metasfresh/issues/6807) Date Issue in Shipment Schedule quick Edit
  * [#6808](https://github.com/metasfresh/metasfresh/issues/6808) Materialentnahme with kg palettes creates extra 0.001Kg TU
  * [#6822](https://github.com/metasfresh/metasfresh/issues/6822) Translation: 'Transportation Order' / 'Bill of Lading'
  * [#6848](https://github.com/metasfresh/metasfresh/issues/6848) Attribute ID shall not be shown in Attribute Editor/ Attribute Button
  * [#6862](https://github.com/metasfresh/metasfresh/issues/6862) Customer complaint: Error when starting Action "Vorgang anlegen"
  * [#6868](https://github.com/metasfresh/metasfresh/issues/6868) Packing Instruction selectable that does not fit to Businesspartner
  * [#6883](https://github.com/metasfresh/metasfresh/issues/6883) Make 'Stammdaten Mutationsprotokol' report display table name on multiple lines if it doesn't fit on one
  * [#6888](https://github.com/metasfresh/metasfresh/issues/6888) BOM verified already set after copy of Product
  * [#6892](https://github.com/metasfresh/metasfresh/issues/6892) Jasper: Liefervertrag adjustments
  * [#6921](https://github.com/metasfresh/metasfresh/issues/6921) Set Parent and Seqno in C_ElementValue when importing accounts
  * [#6938](https://github.com/metasfresh/metasfresh/issues/6938) Jasper Pricelist & Pricelist comparison correct digits in prices
  * [#6965](https://github.com/metasfresh/metasfresh/issues/6965) WEBUI_Fact_Acct_Repost_ViewRows - DocumentToRepost seems to be ignored
  * [#6975](https://github.com/metasfresh/metasfresh/issues/6975) Default LU and Qty not proposed
  * [#6979](https://github.com/metasfresh/metasfresh/issues/6979) Error in workpackage when trying to create invoices

* metasfresh-webui-api-legacy
  * [#1402](https://github.com/metasfresh/metasfresh-webui-api-legacy/pull/1402) Fixing Material Receipt Candidates -> Create Material Receipt error

* metasfresh-webui-frontend-legacy
  * [#2683](https://github.com/metasfresh/metasfresh-webui-frontend-legacy/issues/2683) UI Slower since last Redux refactoring
  * [#2685](https://github.com/metasfresh/metasfresh-webui-frontend-legacy/issues/2685) Checkbox filter with false value not visible in active filters captions
  * [#2691](https://github.com/metasfresh/metasfresh-webui-frontend-legacy/issues/2691) Frontend doesn't correctly evaluate processResult with type=openview

* metasfresh-e2e-legacy
  * [#392](https://github.com/metasfresh/metasfresh-e2e-legacy/pull/392) Fix new failing tests - investigate what introduced them

# metasfresh 5.144
## Features
* metasfresh
  * [#6403](https://github.com/metasfresh/metasfresh/issues/6403) Avoid memory problems while exporting big datasets to excel
  * [#6393](https://github.com/metasfresh/metasfresh/issues/6393) Generating delivery days for >1 tour not working

* metasfresh-webui-api
  * [#1394](https://github.com/metasfresh/metasfresh-webui-api/issues/1394) layout element: provide maxLength for Text and LongText fields

## Fixes
* metasfresh
  * [#6364](https://github.com/metasfresh/metasfresh/issues/6364) Fixes/ adjustments: Excel Sales Order adjustments
  * [#6376](https://github.com/metasfresh/metasfresh/issues/6376) Avoid empty text for packing material in Product specifications
  * [#6382](https://github.com/metasfresh/metasfresh/issues/6382) Identifiers are swapped for Requests and Invoices
  * [#6390](https://github.com/metasfresh/metasfresh/issues/6390) Fix User Queries with dates throwing error
  * [#6405](https://github.com/metasfresh/metasfresh/issues/6405) Shipment dispo: cache invalidate when mass updating the records

* metasfresh-webui-frontend
  * [#2556](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2556) make sure the view filters are displayed exactly in the same order we have them in the layout

# metasfresh 5.143
## Features
* metasfresh
  * [#6346](https://github.com/metasfresh/metasfresh/issues/6346) Recording of customer complaints from Documents in the Shipment window
  * [#6354](https://github.com/metasfresh/metasfresh/issues/6354) Create a process that allows to set a parent folder for an account

## Fixes
* metasfresh
  * [#6348](https://github.com/metasfresh/metasfresh/issues/6348) NPE when reactivating Sales Order
  * [#6359](https://github.com/metasfresh/metasfresh/issues/6359) NPE in invoice batch entry for partners allowed to campaign prices
  * [#6363](https://github.com/metasfresh/metasfresh/issues/6363) Sales Order: Other product not found in Pricelist
  * [#6370](https://github.com/metasfresh/metasfresh/issues/6370) Paymentterm not taken properly when creating order from Phoneschedule

# metasfresh 5.142
## Features
* metasfresh
  * [#6298](https://github.com/metasfresh/metasfresh/issues/6298) Migrate `AD_Org_ID` process parameter to `Search` from whatever it is now
  * [#6311](https://github.com/metasfresh/metasfresh/issues/6311) Rename jasper report Revisionsstelle Geschäftspartner to Stammdaten Mutationsprotokoll
  * [#6328](https://github.com/metasfresh/metasfresh/issues/6328) ESR Import + processing autom. after upload via drag&drop

## Fixes
* metasfresh
  * [#6231](https://github.com/metasfresh/metasfresh/issues/6231) UOM related error in invoice candidate updates
  * [#6331](https://github.com/metasfresh/metasfresh/issues/6331) The Greeting of the contact is not translated in address block

* metasfresh-webui-frontend
  * [#2640](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2640) DevTools failed to parse SourceMap error

# metasfresh 5.141
## Features
* metasfresh
  * [#6190](https://github.com/metasfresh/metasfresh/issues/6190) Jasper Report: Summary and balance list - Summen- und Saldenliste
  * [#6283](https://github.com/metasfresh/metasfresh/issues/6283) Implement SEPA Direct Debit
  * [#6289](https://github.com/metasfresh/metasfresh/issues/6289) Bankstatement improvements
  * [#6291](https://github.com/metasfresh/metasfresh/issues/6291) User in generated invoice must be active

* metasfresh-parent
  * [#42](https://github.com/metasfresh/metasfresh-parent/pull/42) Use binary git after a test which i made yesterday

# metasfresh 5.140
## Features
* metasfresh
  * [#6191](https://github.com/metasfresh/metasfresh/issues/6191) Jasper: Customer Top Revenue
  * [#6255](https://github.com/metasfresh/metasfresh/issues/6255) Create functions for easily creating default accounts fro M_Produc_category, M_Product, C_BP_Group and C_Bpartner

## Fixes
* metasfresh
  * [#6214](https://github.com/metasfresh/metasfresh/issues/6214) Jasper Report: Customer/ Vendor Kontenblatt (Account details)
  * [#6263](https://github.com/metasfresh/metasfresh/issues/6263) Error logging dunnings in DocOutBoundLog
  * [#6277](https://github.com/metasfresh/metasfresh/issues/6277) Issues with payment endpoint

* metasfresh-webui-frontend
  * [#2626](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2626) Again: Orderlines only displayed after refresh

# metasfresh 5.139
## Features
* metasfresh
  * [#6133](https://github.com/metasfresh/metasfresh/issues/6133) Jasper: Customer Product Statistic
  * [#6148](https://github.com/metasfresh/metasfresh/issues/6148) Jasper Report: Profit & Loss Report
  * [#6150](https://github.com/metasfresh/metasfresh/issues/6150) Jasper: Product Top Sales
  * [#6154](https://github.com/metasfresh/metasfresh/issues/6154) Backend: Send new object in JSON of available docaction dropdowns for VOID Action
  * [#6156](https://github.com/metasfresh/metasfresh/issues/6156) Add clone action for "Transportation Order" window.
  * [#6167](https://github.com/metasfresh/metasfresh/issues/6167) Rename 'Verrechnung Billcare' process
  * [#6168](https://github.com/metasfresh/metasfresh/issues/6168) Enhance campaign pricing to apply also based on pricing system
  * [#6182](https://github.com/metasfresh/metasfresh/issues/6182) Add IBAN structure for DK
  * [#6197](https://github.com/metasfresh/metasfresh/issues/6197) Adjust timeout so that big report to be able to run
  * [#6201](https://github.com/metasfresh/metasfresh/issues/6201) Support packing instructions for invoice line 'Batch entry'
  * [#6207](https://github.com/metasfresh/metasfresh/issues/6207) Minor adjustments to customs invoice document
  * [#6216](https://github.com/metasfresh/metasfresh/issues/6216) Filter for Virtual Column
  * [#6219](https://github.com/metasfresh/metasfresh/issues/6219) Product Price creation for Price = 0
  * [#6223](https://github.com/metasfresh/metasfresh/issues/6223) Material Tracking Copy action

* metasfresh-webui-api
  * [#1363](https://github.com/metasfresh/metasfresh-webui-api/issues/1363) Add possibility to turn off 'Area Search' filter

## Fixes
* metasfresh
  * [#6157](https://github.com/metasfresh/metasfresh/issues/6157) Order: when setting the DocType, consider the default one first
  * [#6174](https://github.com/metasfresh/metasfresh/issues/6174) Don't use delivery day with wrong bpartner
  * [#6215](https://github.com/metasfresh/metasfresh/issues/6215) Exclude migration-cli from reports service

* metasfresh-webui-api
  * [#6174](https://github.com/metasfresh/metasfresh/issues/6175) webui-api: fix the webui.view.itemsSelected.caption AD_Message

# metasfresh 5.138
## Features
* metasfresh
  * [#6065](https://github.com/metasfresh/metasfresh/issues/6065) WebUI Window adjustment, Printing Queue
  * [#6072](https://github.com/metasfresh/metasfresh/issues/6072) Tour in Purchase Order, Purchase Order as Transport order Lines for fetch entries
  * [#6120](https://github.com/metasfresh/metasfresh/issues/6120) Make shipping more robust to certain use-cases
  * [#6139](https://github.com/metasfresh/metasfresh/issues/6139) Soothe FUD regarding user login

* metasfresh-parent
  * [#38](https://github.com/metasfresh/metasfresh-parent/pull/38) Minor parent pom clienup

## Fixes
* metasfresh
  * [#6125](https://github.com/metasfresh/metasfresh/issues/6125) Docaction Permission not taken properly for Bank Statement
  * [#6129](https://github.com/metasfresh/metasfresh/issues/6129) Product Name change leads to update of all Translations already entered
  * [#6130](https://github.com/metasfresh/metasfresh/issues/6130) BPartner Import bugfixes
  * [#6137](https://github.com/metasfresh/metasfresh/pull/6137) Avoid NPE in ESRInfoProviderImpl

# metasfresh 5.137
## Features
* metasfresh
  * [#6054](https://github.com/metasfresh/metasfresh/pull/6054) only set C_OLCand.ProductDescription if different from product-name
  * [#6077](https://github.com/metasfresh/metasfresh/issues/6077) Add grouping warehouse in Bestellkontrolle report
  * [#6085](https://github.com/metasfresh/metasfresh/issues/6085) Presetting of Qty CU and default LU in action receipt
  * [#6098](https://github.com/metasfresh/metasfresh/pull/6098) bump up lombok version to 1.18.10

* metasfresh-edi
  * [#8](https://github.com/metasfresh/metasfresh-edi/issues/8) EDI - add switch to disable delivery variance element

* metasfresh-parent
  * [#5](https://github.com/metasfresh/metasfresh-parent/issues/5) Generate git.properties

# metasfresh 5.136
## Features
* metasfresh
  * [#6045](https://github.com/metasfresh/metasfresh/issues/6045) Price Calculation as % of margin
  * [#6106](https://github.com/metasfresh/metasfresh/issues/6106) Accounting misc fixes

* metasfresh-webui-api
  * [#1340](https://github.com/metasfresh/metasfresh-webui-api/issues/1340) Implement GET /rest/api/window/{windowId}/{documentId}/{tabId}?ids=comma separated rowIds

## Fixes
* metasfresh
  * [#6064](https://github.com/metasfresh/metasfresh/issues/6064) Printing a Customs Invoice returns wrong number of decimals for kg quantity

# metasfresh 5.135
## Features
* metasfresh
  * [#5949](https://github.com/metasfresh/metasfresh/issues/5949) Automatic Shipping Label Printing (DPD)
  * [#5965](https://github.com/metasfresh/metasfresh/pull/5965) Improve logging in pricing rules
  * [#6001](https://github.com/metasfresh/metasfresh/issues/6001) measure and log how much each model interceptor took
  * [#6028](https://github.com/metasfresh/metasfresh/issues/6028) Extract quotation logic in jasper-DB-functions
  * [#6032](https://github.com/metasfresh/metasfresh/issues/6032) Excel SQL Process with qty of invoices per daterange
  * [#6035](https://github.com/metasfresh/metasfresh/issues/6035) Make C_UOM editable in C_InvoiceLine
  * [#6048](https://github.com/metasfresh/metasfresh/issues/6048) Improve Price Schema Excel Export
  * [#6057](https://github.com/metasfresh/metasfresh/issues/6057) Show BOM in window Stücklistenbestandteile

* metasfresh-parent
  * [#33](https://github.com/metasfresh/metasfresh-parent/pull/33) Add git infos to each build artefact

## Fixes
* metasfresh 
  * [#6030](https://github.com/metasfresh/metasfresh/issues/6030) Report Average Product Prices: Negate in case of Credit Memo
  * [#6031](https://github.com/metasfresh/metasfresh/issues/6031) Update line-schema-id if updated in parent record

* metasfresh-webui-api
  * [#1343](https://github.com/metasfresh/metasfresh-webui-api/issues/1343) Add an unit test for how the selected rows ids are sent as parameters

# metasfresh 5.134
## Features
* metasfresh
  * [#5940](https://github.com/metasfresh/metasfresh/issues/5940) Packing Instruction in Batch Entry
  * [#5987](https://github.com/metasfresh/metasfresh/issues/5987) Multiple Customs Invoices for the same Shipment
  * [#5992](https://github.com/metasfresh/metasfresh/issues/5992) Improve DESADV Packs window
  * [#6007](https://github.com/metasfresh/metasfresh/issues/6007) UOM Conversion check in Product Prices
  * [#6024](https://github.com/metasfresh/metasfresh/issues/6024) Make sure shipto companyname is transferred to c_bpartner_location.bpartnername

* edi
  * [#6](https://github.com/metasfresh/metasfresh-edi/issues/6) STEPcom EDI - Convert between input charset and UTF-8
  * [#7](https://github.com/metasfresh/metasfresh-edi/issues/7) STEPcom EDI - Support customizable output filename prefices

## Fixes
* metasfresh
  * [#5931](https://github.com/metasfresh/metasfresh/issues/5931) ESR Import Hashvalue after double upload
  * [#6006](https://github.com/metasfresh/metasfresh/issues/6006) Picklist cannot be printed
  * [#6014](https://github.com/metasfresh/metasfresh/issues/6014) Compute properly sum catch weight in customs invoice document
  * [#6017](https://github.com/metasfresh/metasfresh/issues/6017) Drop the wrong duplicate PayPal payment rule

# metasfresh 5.133
## Features
* metasfresh
  * [#5885](https://github.com/metasfresh/metasfresh/issues/5885) Tour dependent adjustments
  * [#5896](https://github.com/metasfresh/metasfresh/issues/5896) SSCC label printing on Zebra printers
  * [#5915](https://github.com/metasfresh/metasfresh/issues/5915) Support recording of weight also for TopLevel-CUs
  * [#5922](https://github.com/metasfresh/metasfresh/issues/5922) Customer Order Excel in WebUI
  * [#5929](https://github.com/metasfresh/metasfresh/issues/5929) Set by default metasfresh C_Element to IsNaturalAccount ='Y'
  * [#5933](https://github.com/metasfresh/metasfresh/issues/5933) accounting: display Posted flag in ALL documents
  * [#5958](https://github.com/metasfresh/metasfresh/pull/5958) SQL Process Excel Download: List all orderlines that could not be delivered although due
  * [#5970](https://github.com/metasfresh/metasfresh/issues/5970) Process to update AD_User_Record_Access from BPartner Hierarchy
  * [#5972](https://github.com/metasfresh/metasfresh/issues/5972) Set async connection pool size to 1

## Fixes
* metasfresh
  * [#4879](https://github.com/metasfresh/metasfresh/issues/4870) Shipment schedule not updated when asi in orderline is updated
  * [#5924](https://github.com/metasfresh/metasfresh/issues/5924) Accounting/ Costing Issues
  * [#5947](https://github.com/metasfresh/metasfresh/issues/5947) DocActions displayed incorrectly
  * [#5960](https://github.com/metasfresh/metasfresh/issues/5960) Shipmentschedule not updated after order reactivate and re-complete
  * [#5962](https://github.com/metasfresh/metasfresh/issues/5962) Bug at material receipts with weight-unrelated products

# metasfresh 5.132
## Features
* metasfresh
  * [#5800](https://github.com/metasfresh/metasfresh/issues/5800) Add Payment Type, Shipper, Sales Partner to order candidate endpoint
  * [#5856](https://github.com/metasfresh/metasfresh/issues/5856) Add payment rest endpoint
  * [#5865](https://github.com/metasfresh/metasfresh/issues/5865) Picklist not working: "Type not supported: UNALLOCABLE"
  * [#5887](https://github.com/metasfresh/metasfresh/issues/5887) Additional Invoice Information
  * [#5888](https://github.com/metasfresh/metasfresh/issues/5888) Picklist ordered by locator name + dimensions
  * [#5895](https://github.com/metasfresh/metasfresh/issues/5895) Create Window for managing Manufactoring Workflow
  * [#5900](https://github.com/metasfresh/metasfresh/issues/5900) product proposals: Copy product price from other price list shall set IsInvalidPrice=N
  * [#5901](https://github.com/metasfresh/metasfresh/issues/5901) Automatically create C_ValidCombination(s) when a new C_ElementValue is created
  * [#5906](https://github.com/metasfresh/metasfresh/issues/5906) Add poreference field in the sql function to get data for sales order report
  * [#5908](https://github.com/metasfresh/metasfresh/issues/5908) SQL Process for BPartner Products as Excel List
  * [#5912](https://github.com/metasfresh/metasfresh/issues/5912) Read documentno field in the report for customer invoice with credit memo
  * [#5917](https://github.com/metasfresh/metasfresh/issues/5917) Product price not found if ASI was added to order line
* metasfresh-webui-api
  * [#1330](https://github.com/metasfresh/metasfresh-webui-api/issues/1330) Reduce the number of websocket events we are sending to frontend
  * [#2469](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2469) Re-fetch tab's actions when the document status changes

* metasfresh-webui-frontend
  * [#2436](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2436) Follow-Up: Customer Proposal List navigation with arrow keys (qty arrows out)

## Fixes
* metasfresh
  * [#5903](https://github.com/metasfresh/metasfresh/issues/5903) Fix country code from de_metas_endcustomer_fresh_reports.Docs_Sales_Invoice_Root

* metasfresh-webui-frontend
  * [#2471](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2471) Attributes cannot be set in orderline grid view
  * [#2477](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2477) Location name seems to get lost when editing the location
  * [#2488](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2488) Add new button doesn't work anymore

# metasfresh 5.131
## Features
* metasfresh
  * [#5850](https://github.com/metasfresh/metasfresh/issues/5850) Add Net Amount and Gross Amount in Partner Window, Tab Request
  * [#5861](https://github.com/metasfresh/metasfresh/issues/5861) Initial Cost Price via Inventory import
  * [#5869](https://github.com/metasfresh/metasfresh/issues/5869) Add Check for isCreditMemo in function Docs_Sales_Invoice_Description
  * [#5880](https://github.com/metasfresh/metasfresh/issues/5880) Support inheriting Attribute from Phantom BOM to order line to support pricing
  * [#5882](https://github.com/metasfresh/metasfresh/issues/5882) migration scripts: avoid logging AD_Preference changes

* metasfresh-webui-frontend
  * [#2475](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2475) Refresh quickActions in both included and parent view when selection changes

## Fixes
* metasfresh
  * [#5874](https://github.com/metasfresh/metasfresh/issues/5874) Reactivate Shipment, update Shipmentline delivery catch weight => does not update invoice candidate
  * [#5878](https://github.com/metasfresh/metasfresh/issues/5878) automatically create native sequence when an AD_Table is created
  * [#5802](https://github.com/metasfresh/metasfresh/issues/5802) Bug in Pricelistversion update for Basepricelists and customer proposals

* metasfreseh-webui-frontend
  * [#2454](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2454) Time not displayed in widgets
  * [#2472](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2472) Purchase order from sales order not working anymore
  * [#2474](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2474) X button not working for several fields

# metasfresh 5.130
## Features
* metasfresh
  * [#5070](https://github.com/metasfresh/metasfresh/issues/5070) Discount Schema Lines in separate window
  * [#5799](https://github.com/metasfresh/metasfresh/issues/5799) Pricelist Schema export-import for Basepricelists
  * [#5806](https://github.com/metasfresh/metasfresh/issues/5806) OLCand - Improve support for TU UOMs
  * [#5824](https://github.com/metasfresh/metasfresh/issues/5824) IBAN Liechtenstein not accepted as Bank Account
  * [#5834](https://github.com/metasfresh/metasfresh/issues/5834) Sales Order recording without Billto Partner
  * [#5840](https://github.com/metasfresh/metasfresh/issues/5840) Allow manual creation of Phonecall Schedule
  * [#5845](https://github.com/metasfresh/metasfresh/issues/5845) Invoice reversal via REST-EP
  * [#5851](https://github.com/metasfresh/metasfresh/issues/5851) Add currency in doc_sales_invoice_root and in doc_sales_order_root functions

* metasfresh-webui-api
  * [#1315](https://github.com/metasfresh/metasfresh-webui-api/issues/1315) Product proposal view: show customer name in header
  * [#1320](https://github.com/metasfresh/metasfresh-webui-api/issues/1320) Payment Allocation Window in WebUI

## Fixes
* metasfresh
  * [#5802](https://github.com/metasfresh/metasfresh/issues/5802) Bug in Pricelistversion update for Basepricelists and customer proposals
  * [#5829](https://github.com/metasfresh/metasfresh/issues/5829) Report aren't working anymore

# metasfresh 5.129
## Features
* metasfresh 
  * [#5626](https://github.com/metasfresh/metasfresh/issues/5626) Support C_OLCands without UOM
  * [#5679](https://github.com/metasfresh/metasfresh/issues/5679) Trading BOM
  * [#5786](https://github.com/metasfresh/metasfresh/issues/5786) Endpoint: get invoice PDF
  * [#5797](https://github.com/metasfresh/metasfresh/issues/5797) Fix DB-function altercolumn to not fail on materialized views
  * [#5801](https://github.com/metasfresh/metasfresh/pull/5801) make invoice candidate updating robust to missing price
  * [#5804](https://github.com/metasfresh/metasfresh/issues/5804) BPartner Name overwrite in BPartner Location
  * [#5814](https://github.com/metasfresh/metasfresh/issues/5814) Introduce C_OrderLine.ExplodedFrom_BOMLine_ID

* metasfresh-webui-api
  * [#1303](https://github.com/metasfresh/metasfresh-webui-api/issues/1303) shipment schedules edit modal: order rows by order and order line
  * [#1305](https://github.com/metasfresh/metasfresh-webui-api/issues/1305) shipment schedule editor: pimp layout + show packing instructions
  * [#1307](https://github.com/metasfresh/metasfresh-webui-api/issues/1307) products proposal: optimize layout for better usability
  * [#1311](https://github.com/metasfresh/metasfresh-webui-api/issues/1311) product proposal: add Description field and make it editable

# metasfresh 5.128
## Features
* metasfresh 
  * [#5430](https://github.com/metasfresh/metasfresh/issues/5430) report server: autodetect and use workspace jasperreports folders
  * [#5637](https://github.com/metasfresh/metasfresh/issues/5637) Add DPD Shipper and DPD integration
  * [#5755](https://github.com/metasfresh/metasfresh/issues/5755) Create endpoint to directly insert invoice candidates
  * [#5774](https://github.com/metasfresh/metasfresh/issues/5774) Invoice candidates sometimes remain "ToUpdate" after the invoice was created
  * [#5776](https://github.com/metasfresh/metasfresh/issues/5776) Distribution Network from Main-Warehouse to Picking Warehouse
  * [#5782](https://github.com/metasfresh/metasfresh/issues/5782) Endpoint: Close Invoice Candidates
  * [#5784](https://github.com/metasfresh/metasfresh/issues/5784) Adjust LU Label
  * [#5789](https://github.com/metasfresh/metasfresh/issues/5789) Don't log migration scripts for AD_Attachment tables
## Fixes
* metasfresh
  * [#5778](https://github.com/metasfresh/metasfresh/issues/5778) Fix potential threadLocalTrxName leakage
  * [#5787](https://github.com/metasfresh/metasfresh/issues/5787) BPartner API error if CreatedBy or UpdatedBy == -1

# metasfresh 5.127
## Features
* metasfresh
  * [#5551](https://github.com/metasfresh/metasfresh/issues/5551) Batchentry Product Name, Stock, Price, best before + additional Field for bestbefore
  * [#5756](https://github.com/metasfresh/metasfresh/issues/5756) Allow Action Prices on Pricing System
  * [#5757](https://github.com/metasfresh/metasfresh/issues/5757) Create endpoint to check the invoice status
  * [#5761](https://github.com/metasfresh/metasfresh/issues/5761)
  * [#5767](https://github.com/metasfresh/metasfresh/issues/5767) Sort by preparation date and order docNo in picking terminal 2

## Fixes
* metasfresh
  * [#5748](https://github.com/metasfresh/metasfresh/issues/5748) HU editor: clearing the Production Date field leads to error
  * [#5772](https://github.com/metasfresh/metasfresh/issues/5772) Cleared out how shall be BPartner, BPartnerLocation and C_Location in AD_OrgInf

# metasfresh 5.126
## Features
* metasfresh
  * [#5664](https://github.com/metasfresh/metasfresh/issues/5664) Rest endpoint which allows the client to create invoices
  * [#5675](https://github.com/metasfresh/metasfresh/issues/5675) Waste (Entsorgung) from Handling Unit Editor and automatic DocType and No
  * [#5710](https://github.com/metasfresh/metasfresh/issues/5710) Modify process of copying windows to copy the tab callouts as well
  * [#5724](https://github.com/metasfresh/metasfresh/issues/5724) Add more data to shipment report functions
  * [#5729](https://github.com/metasfresh/metasfresh/issues/5729) Only show Catch Weight Fields when catch weight calculation (product price)
  * [#5740](https://github.com/metasfresh/metasfresh/issues/5740) Improve Customs Tariff
  * [#5746](https://github.com/metasfresh/metasfresh/issues/5746) Fix Jenkinsfile: make sure the maven repo name is legit
  * [#5754](https://github.com/metasfresh/metasfresh/issues/5754) AD_System.DBVersion: change size to 255

* metasfresh-webui-frontend
  * [#2401](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2401) Implement Google Maps Integration
  * [#2431](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2431) Remove number field's arrows for changing value

## Fixes
* metasfresh
  * [#5749](https://github.com/metasfresh/metasfresh/pull/5749) HU editor: clearing the Production Date field leads to error
  * [#5735](https://github.com/metasfresh/metasfresh/issues/5735) Linenetamt not rounded to currency precision
  * [#5733](https://github.com/metasfresh/metasfresh/issues/5733) Fix importing process

# metasfresh 5.125
## Features
* metasfresh
  * [#5522](https://github.com/metasfresh/metasfresh/issues/5522) Commission calculation
  * [#5566](https://github.com/metasfresh/metasfresh/issues/5566) Add integration with Google Maps
  * [#5611](https://github.com/metasfresh/metasfresh/issues/5611) Add DHL Shipper and DHL integration
  * [#5683](https://github.com/metasfresh/metasfresh/issues/5683) Empties Saldo report per Day

## Fixes
* metasfresh
  * [#5556](https://github.com/metasfresh/metasfresh/issues/5556) Prevent Running Link Organisation Process if Organisation Field is empty
  * [#5666](https://github.com/metasfresh/metasfresh/issues/5666) Freight Cost invoice candidates bug
  * [#5687](https://github.com/metasfresh/metasfresh/issues/5687) Assumption failure: There is no active M_Attribute record with M_Attribute.Value=M_Material_Tracking_ID
  * [#5701](https://github.com/metasfresh/metasfresh/issues/5701) Document no not updated when changing doctype

# metasfresh 5.124
## Features
* metasfresh
  * [#5602](https://github.com/metasfresh/metasfresh/issues/5602) Cashbook Window
  * [#5656](https://github.com/metasfresh/metasfresh/issues/5656) EDI-Tweaks

## Fixes
* metasfresh-webui-frontend
  * [#2370](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2370) Performance imporovement for Grid Views/ Table Views
  
* metasfresh
  * [#5242](https://github.com/metasfresh/metasfresh/issues/5242) Picking Terminal v2: Cannot fully load AllocationRequest
  * [#5606](https://github.com/metasfresh/metasfresh/issues/5606) Payment window calculation of skonto yes/ no when adjusting date
  * [#5628](https://github.com/metasfresh/metasfresh/issues/5628) Partner relations don't work properly in sales order
  * [#5659](https://github.com/metasfresh/metasfresh/issues/5659) Picklist in Picking Terminal v2 automatically picks, but shall not


# metasfresh 5.123
## Features
* metasfresh
  * [#5575](https://github.com/metasfresh/metasfresh/issues/5575) Add `ExternalId` to Product
  * [#5589](https://github.com/metasfresh/metasfresh/issues/5589) New Window for BOM Components & Reference to BOM
  * [#5592](https://github.com/metasfresh/metasfresh/issues/5592) Show warehouse search key value in Grid View
  * [#5609](https://github.com/metasfresh/metasfresh/issues/5609) persistent object: log warning if changing an PO on after new/change
  * [#5616](https://github.com/metasfresh/metasfresh/issues/5616) New Tab Ingredients in Product window
  * [#5620](https://github.com/metasfresh/metasfresh/issues/5620) Set automatically Name field from AD_UI_Element
  * [#5625](https://github.com/metasfresh/metasfresh/issues/5625) Material Tracking - change quality discount base
  * [#5639](https://github.com/metasfresh/metasfresh/issues/5639) Print Picklist from Picking terminal v2
  * [#5645](https://github.com/metasfresh/metasfresh/issues/5645) BOM Components followup - Comment, Change notice and Expected result to be added
  * [#5564](https://github.com/metasfresh/metasfresh/issues/5564) Import Process Performance
  * [#5644](https://github.com/metasfresh/metasfresh/issues/5644) Action: Update Invoice Location and contact for all selected lines
  * [#5649](https://github.com/metasfresh/metasfresh/issues/5649) GTIN in Product window
  * [#5652](https://github.com/metasfresh/metasfresh/issues/5652) OLCand - support requests without BPartner-Location

## Fixes
* metasfresh
  * [#5598](https://github.com/metasfresh/metasfresh/issues/5598) NPE Async for sending email from DocOutbound
  * [#5599](https://github.com/metasfresh/metasfresh/issues/5599) No invoice from Picking Terminal 2: NetAmtToInvoice checksum not match
  * [#5600](https://github.com/metasfresh/metasfresh/issues/5600) No invoice bc of QuantitiesUOMNotMatchingExpection
  * [#5613](https://github.com/metasfresh/metasfresh/issues/5613) Partner relations for invoice location allows only one invoice receipient
  * [#5615](https://github.com/metasfresh/metasfresh/pull/5615) Ad_tab fix `ModelValidator.TYPE_AFTER_NEW, ModelValidator.TYPE_AFTER_CHANGE` error
  * [#5617](https://github.com/metasfresh/metasfresh/pull/5617) bugfix wrt bpartner-lookup just via GLN
  * [#5629](https://github.com/metasfresh/metasfresh/issues/5629) Can't create a new order
  
* metasfresh-webui-api
  * [#1270](https://github.com/metasfresh/metasfresh-webui-api/issues/1270) Org-ID not found Callout error

* metasfresh-webui-frontend
  * [#2394](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2394) Rounded corners missing in mandatory fields
  * [#2393](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2393) Sales Order Line: fix batch entry layout
  * [#2403](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2403) Widgets not properly automatically updated
  * [#2405](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2405) Fix sorting in tabs-tables

# metasfresh 5.122
## Features
* metasfresh
  * [#2518](https://github.com/metasfresh/metasfresh/issues/2518) Add Zahlung einlesen in Action menu for purchase invoice
  * [#5569](https://github.com/metasfresh/metasfresh/issues/5569) Mandatory Field in Purchase Order: Warehouse ID
  * [#5587](https://github.com/metasfresh/metasfresh/issues/5587) New Window for Packvorschrift (CU-TU) Standalone

## Fixes
* metasfresh-webui-frontend
  * [#2364](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2364) Organisation and client field misalligned
  * [#2367](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2367) Adjustments for dates in filters
  * [#2383](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2383) Fix filter widgets typing
  * [#2385](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2385) Border radius disturbing on Lookup Fields
  * [#2391](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2391) Date range picker is not working anymore in Action parms

# metasfresh 5.121

## Features
* metasfresh
  * [#5443](https://github.com/metasfresh/metasfresh/issues/5443) Have dedicated Window for UI Elements
  * [#5444](https://github.com/metasfresh/metasfresh/issues/5444) Have dedicated window for organisational master data business partner
  * [#5523](https://github.com/metasfresh/metasfresh/pull/5523) Add role update and process documents to webui menu tree
  * [#5527](https://github.com/metasfresh/metasfresh/pull/5527) Lookup widget instead of dropdown
  * [#5538](https://github.com/metasfresh/metasfresh/pull/5538) Pricesystem shall be search widget not dropdown
  * [#5540](https://github.com/metasfresh/metasfresh/issues/5540) Implement receipt CU Label
  * [#5544](https://github.com/metasfresh/metasfresh/issues/5544) Picking with bestBefore shortest/ longest option
  * [#5549](https://github.com/metasfresh/metasfresh/pull/5549) New Window: Unposted Documents
  * [#5554](https://github.com/metasfresh/metasfresh/pull/5554) New Window in WebUI for Matched Invoices
  * [#5555](https://github.com/metasfresh/metasfresh/issues/5555) procurement webapp: Info Page: show HTML text instead of PREformated text

## Fixes
* metasfresh
  * [#5529](https://github.com/metasfresh/metasfresh/issues/5529) Bestellkontrolle (Barcode): Packing Instruction cut off
  * [#5550](https://github.com/metasfresh/metasfresh/pull/5550) Avoid starting main spring boot classes if they are not started standalone
  * [#5558](https://github.com/metasfresh/metasfresh/issues/5558) webapi log is flooded with various warnings/errors
  * [#5574](https://github.com/metasfresh/metasfresh/issues/5574) Error updating M_ShipmentSchedule that references a flatrate term

* metasfresh-webui-api
  * [#1252](https://github.com/metasfresh/metasfresh-webui-api/issues/1252) Org Timezone Berlin: Promised Date still dependent on local timezone
  * [#1257](https://github.com/metasfresh/metasfresh-webui-api/pull/1257) Organisation as Search Widget

# metasfresh 5.120

## Features
* metasfresh
  * [#5487](https://github.com/metasfresh/metasfresh/issues/5487) Allow Copy for M_ProductPrice
  * [#5519](https://github.com/metasfresh/metasfresh/pull/5519) Sektion als Suchfeld

# Fixes
* metasfresh
  * [#5506](https://github.com/metasfresh/metasfresh/issues/5506) Dunning Disposition Action to set Dunning Grace does not update existing Dates
  * [#5514](https://github.com/metasfresh/metasfresh/issues/5514) forum-datenaustausch.ch only update biller masterdata
  * [#5495](https://github.com/metasfresh/metasfresh/issues/5495) allow material dispo to run within app

* metasfresh-webui-frontend
  * [#2359](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2359) Date filter problem in Material Cockpit
  * [#2835](https://github.com/metasfresh/me03/issues/2835) "Created" date looking weird
  * [#2844](https://github.com/metasfresh/me03/issues/2844) Record stays on same position after going next page after grid edit


# metasfresh 5.119

## Features
* metasfresh
  * [#4352](https://github.com/metasfresh/metasfresh/issues/4352) WebUI Project and ProjectType Window
  * [#5384](https://github.com/metasfresh/metasfresh/issues/5384) Catch Weight invoicing
  * [#5450](https://github.com/metasfresh/metasfresh/issues/5450) New Action Price update für basepricelist and customer pricelist
  * [#5453](https://github.com/metasfresh/metasfresh/issues/5453) Data Import REST endpoints
  * [#5461](https://github.com/metasfresh/metasfresh/issues/5461) Have a way to fix native sequence problems from metasfresh
  * [#5465](https://github.com/metasfresh/metasfresh/issues/5465) requests: when sales rep is changed, notify the new sales rep about the change
  * [#5470](https://github.com/metasfresh/metasfresh/issues/5470) Copy discount schema breaks of product - new process
  * [#5471](https://github.com/metasfresh/metasfresh/issues/5471) Date Filter in Payment Window
  * [#5478](https://github.com/metasfresh/metasfresh/issues/5478) Allow copy with details for Payment
  * [#5479](https://github.com/metasfresh/metasfresh/issues/5479) Ändert MF etwas beim external_factor im xml an den Kanton (KT_xx)
  * [#5494](https://github.com/metasfresh/metasfresh/issues/5494) Change inventory import for the generic case

* metasfresh-webui-frontend
  * [#2350](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2350) Respect new lines in webui texts

## Fixes
* metasfresh
  * [#5466](https://github.com/metasfresh/metasfresh/issues/5466) Assumption failure: repoId > 0 but it was 0 Additional parameters in notifications
  * [#5477](https://github.com/metasfresh/metasfresh/issues/5477) NullPointer Exception beim Import von Rückweisungen der Krankenkasse
  
* metasfresh-webui-frontend
  * [#2351](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2351) The date is displayed differently in grid view vs. single view


# metasfresh 5.118

# Features
* metasfresh
  * [#5423](https://github.com/metasfresh/metasfresh/issues/5423) Drafted PP Orders shall not create demands
  * [#5440](https://github.com/metasfresh/metasfresh/issues/5440) Easy shipment candidate recording (Modal Overlay)
  * [#5447](https://github.com/metasfresh/metasfresh/issues/5447) Optionally include C_Location changes in parent record's changelog
  * [#5457](https://github.com/metasfresh/metasfresh/issues/5457) MaterialTracking - Support regular PP_Orders with heterogenous components
  * [#5471](https://github.com/metasfresh/metasfresh/issues/5471) Date Filter in Payment Window

* metasfresh-webui-api
  * [#1245](https://github.com/metasfresh/metasfresh-webui-api/issues/1245) webui cache reset: don't invalidate new/changed documents

## Fixes
* metasfresh 
  * [#5380](https://github.com/metasfresh/metasfresh/issues/5380) Fix timezone issues

* metasfresh-webui-api
  * [#1248](https://github.com/metasfresh/metasfresh-webui-api/issues/1248) webui: don't apply role permissions when loading layout fields

# metasfresh 5.117

## Features
* metasfresh
  * [#5426](https://github.com/metasfresh/metasfresh/issues/5426) Implement MetasfreshBeanNameGenerator to avoid spring bean name collisions in case of model Interceptors

* metasfresh-e2e
  * [#125](https://github.com/metasfresh/metasfresh-e2e/issues/125) Open Handling Unit Editor
  * [#145](https://github.com/metasfresh/metasfresh-e2e/issues/145) Purchase order from sales order
  * [#210](https://github.com/metasfresh/metasfresh-e2e/issues/210) Create material receipt with quality issue

## Fixes
* metasfresh
  * [#5193](https://github.com/metasfresh/metasfresh/issues/5193) Error when trying to issue for >1 component in manufacturing


* metasfresh-webui-api
  * [#2334](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2334) Error when layout shortcuts is not defined

# metasfresh 5.116

## Features
* metasfresh-e2e
  * [#116](https://github.com/metasfresh/metasfresh-e2e/issues/116) Create new tour and transportation order
  * [#136](https://github.com/metasfresh/metasfresh-e2e/issues/136) Change product price (product window) and use it
  * [#153](https://github.com/metasfresh/metasfresh-e2e/issues/153) Change warehouse in material receipt candidate
  * [#229](https://github.com/metasfresh/metasfresh-e2e/issues/229) Create new Shipper
  * [#231](https://github.com/metasfresh/metasfresh-e2e/issues/231) Adapt Tourversion
  * [#248](https://github.com/metasfresh/metasfresh-e2e/issues/248) Create Disposal from Handling Unit Editor
  * [#277](https://github.com/metasfresh/metasfresh-e2e/issues/277) Create Vendor Return
  * [#278](https://github.com/metasfresh/metasfresh-e2e/issues/278) Create pricelist schema
  * [#279](https://github.com/metasfresh/metasfresh-e2e/issues/279) Create new pricelist version using a pricelist schema
  * [#280](https://github.com/metasfresh/metasfresh-e2e/issues/280) Add a product to a pricelist schema and create a new PLV

# metasfresh 5.115

## Features
* metasfresh
  * [#5411](https://github.com/metasfresh/metasfresh/issues/5411) Reset auth token for Json Reports user on each app-server-start
  * [#5382](https://github.com/metasfresh/metasfresh/issues/5382) Show reversal_id in advanced edit of empties return / receive

* metasfresh-e2e
  * [#213](https://github.com/metasfresh/metasfresh-e2e/issues/213) Reverse Empties Return
  * [#233](https://github.com/metasfresh/metasfresh-e2e/issues/233) Change product prices and add a new one

## Fixes
* metasfresh-webui-frontend
  * [#2325](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2325) frontend patches too much in quick input field

# metasfresh 5.114

## Features
* metasfresh
  * [#5041](https://github.com/metasfresh/metasfresh/issues/5041) Implement Paypal Plus support
  * [#5392](https://github.com/metasfresh/metasfresh/issues/5392) Discount Rows new action "copy to discount schema" for selected rows
  * [#5405](https://github.com/metasfresh/metasfresh/issues/5405) New Subtab in Product for Campaign prices

* metasfresh-e2e
  * [#108](https://github.com/metasfresh/metasfresh-e2e/issues/108) Create purchase order with orderline, complete / reactivate / complete again
  * [#155](https://github.com/metasfresh/metasfresh-e2e/issues/155) Create purchase order with orderline, complete / reactivate / change qties and price in orderline / complete again
  * [#211](https://github.com/metasfresh/metasfresh-e2e/issues/211) Create Empties Returns
  * [#212](https://github.com/metasfresh/metasfresh-e2e/issues/212) Reactivate and change Empties Return
  * [#230](https://github.com/metasfresh/metasfresh-e2e/issues/230) Create new Tour and Tourversion
  * [#232](https://github.com/metasfresh/metasfresh-e2e/issues/232) Create Delivery Days

## Fixes
* metasfresh
  * [#5400](https://github.com/metasfresh/metasfresh/issues/5400) Error when opening Picking Terminal prototype

* metasfresh-webui-frontend
  * [#1822](https://github.com/metasfresh/me03/issues/1822) Fix decimal comma in Qty Fields

# metasfresh 5.113

## Features
* metasfresh
  * [#5364](https://github.com/metasfresh/metasfresh/issues/5364) BPartner REST-API - Add Support for additional core fields
  * [#5390](https://github.com/metasfresh/metasfresh/pull/5390) Add Quality Issue warehouse filter in Warehouse list page
  * [#5370](https://github.com/metasfresh/metasfresh/issues/5370) Introduce more webui WidgetSizes (XL, XXL)

* metasfresh-webui-frontend
  * [#2304](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2304) Picking Terminal (Prototype): not all picking slots not displayed / close when clicking outside
  * [#2307](https://github.com/metasfresh/metasfresh-webui-frontend/pull/2307) Set precision to 2 digits for `CableLength` field

* metasfresh-e2e
  * [#46](https://github.com/metasfresh/metasfresh-e2e/issues/46) Create test: warehouse
  * [#121](https://github.com/metasfresh/metasfresh-e2e/issues/121) Create new Stock Control Purchase
  * [#126](https://github.com/metasfresh/metasfresh-e2e/issues/126) Create Empties Receive
  * [#129](https://github.com/metasfresh/metasfresh-e2e/issues/129) Create Dunning Candidates
  * [#130](https://github.com/metasfresh/metasfresh-e2e/issues/130) Create Dunning Documents
  * [#132](https://github.com/metasfresh/metasfresh-e2e/issues/132) Void sales invoice and invoice the billing candidates again
  * [#162](https://github.com/metasfresh/metasfresh-e2e/issues/162) Create credit memo Vendor (Lieferant)

# metasfresh 5.112

## Features
* metasfresh
  * [#5257](https://github.com/metasfresh/metasfresh/issues/5257) Data Migration for Data Entry 
  * [#5353](https://github.com/metasfresh/metasfresh/issues/5353) Enable "Bank" import

* metasfresh-e2e
  * [#85](https://github.com/metasfresh/metasfresh-e2e/issues/85) Create new Packing Instruction / Packing Instruction Version
  * [#134](https://github.com/metasfresh/metasfresh-e2e/issues/134) Create credit memo price difference for sales invoice
  * [#135](https://github.com/metasfresh/metasfresh-e2e/issues/135) Create credit memo deliver difference for sales invoice
  * [#152](https://github.com/metasfresh/metasfresh-e2e/issues/152) Change shipment date and date ready in shipment schedule
  * [#188](https://github.com/metasfresh/metasfresh-e2e/pull/188) move defunct specs into dedicated folder
  * [#189](https://github.com/metasfresh/metasfresh-e2e/issues/189) Create Nachbelastung Mengendifferenz for sales invoice
  * [#190](https://github.com/metasfresh/metasfresh-e2e/issues/190) Create Adjustment Charge (Nachbelastung Preisdifferenz) for sales invoice

* metasfresh-webui-frontend
  * [#1740](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1740) email Editor Adress Lookup behavior

## Fixes
* metasfresh
  * [#5346](https://github.com/metasfresh/metasfresh/issues/5346) Pricing Condition fixes

* metasfresh-webui-frontend
  * [#2292](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2292) Doubleclick does not work on mobile (iOS)
  * [#2308](https://github.com/metasfresh/metasfresh-webui-frontend/pull/2308) Dev cypress run hangs

# metasfresh 5.111

## Features
* metasfresh
  * [#5350](https://github.com/metasfresh/metasfresh/issues/5350) Show Referenced Invoice in sales invoice advanced dialog
  * [#5343](https://github.com/metasfresh/metasfresh/issues/5343) New Customer Layout for Produktionskontrolle
  * [#5345](https://github.com/metasfresh/metasfresh/issues/5345) Comma does not work in Attribute value

* metasfresh-webui-api
  * [#1219](https://github.com/metasfresh/metasfresh-webui-api/issues/1219) Make internal names cypress friendly

* metasfresh-e2e
  * [#26](https://github.com/metasfresh/metasfresh-e2e/issues/26) Create Test: set packing item in product window
  * [#77](https://github.com/metasfresh/metasfresh-e2e/issues/77) Create new Packing Material
  * [#111](https://github.com/metasfresh/metasfresh-e2e/issues/111) Create a manual payment
  * [#137](https://github.com/metasfresh/metasfresh-e2e/issues/137) Sales order to shipment to invoice

## Fixes
* metasfresh
  * [#5351](https://github.com/metasfresh/metasfresh/issues/5351) Can't save Print Format properly

# metasfresh 5.110

## Features
* metasfresh
  * [#5273](https://github.com/metasfresh/metasfresh/issues/5273) BPartner REST-API
  * [#5316](https://github.com/metasfresh/metasfresh/issues/5316) C_DocOutbound - improve mail attachment file name
  * [#5328](https://github.com/metasfresh/metasfresh/issues/5328) PP_Order.C_Project_ID virtual column
  * [#5332](https://github.com/metasfresh/metasfresh/issues/5332) Extend Jasper API to run reports using JSON data source
  * [#5334](https://github.com/metasfresh/metasfresh/issues/5334) REST-API - add updated-timestamp to all result objects

* metasfresh-webui-frontend
  * [#2156](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2156) Modal views: shall be easily editable without using mouse

* metasfresh-e2e
  * [#71](https://github.com/metasfresh/metasfresh-e2e/issues/71) Create new BOM
  * [#72](https://github.com/metasfresh/metasfresh-e2e/issues/72) Create new bank
  * [#122](https://github.com/metasfresh/metasfresh-e2e/issues/122) Create GL Journal entry and change posting type
  * [#124](https://github.com/metasfresh/metasfresh-e2e/issues/124) Create new cost center
  * [#127](https://github.com/metasfresh/metasfresh-e2e/issues/127) Create quality note


## fixes
* metasfresh-e2e
  * [#160](https://github.com/metasfresh/metasfresh-e2e/issues/160) Fix isChecked command again

# metasfresh 5.108
## Features
* metasfresh
  * [#5233](https://github.com/metasfresh/metasfresh/issues/5233) Separate eMail Text for Notifications

* metasfresh-e2e
  * [#92](https://github.com/metasfresh/metasfresh-e2e/issues/92) Cypress tests shall not be sensitive to menu language
  * [#100](https://github.com/metasfresh/metasfresh-e2e/issues/100) Create a new user and set a password
  * [#104](https://github.com/metasfresh/metasfresh-e2e/issues/104) Create command for selecting a date from calendar icon

## Fixes
* metasfresh
  * [#5313](https://github.com/metasfresh/metasfresh/issues/5313) Automatischer Debitorenlisten-Export mit falschen Formaten
  * [#5296](https://github.com/metasfresh/metasfresh/issues/5296) Exception on invoicing an invoice candidate

## Fixes

# metasfresh 5.107
## Features
* metasfresh
  * [#5204](https://github.com/metasfresh/metasfresh/issues/5204) On-the-fly auto-allocate available HUs while creating shipments
  * [#5208](https://github.com/metasfresh/metasfresh/issues/5208) Attribute Age automatism
  * [#5210](https://github.com/metasfresh/metasfresh/issues/5210) Customs Document
  * [#5231](https://github.com/metasfresh/metasfresh/issues/5231) Import Replenishments
  * [#5237](https://github.com/metasfresh/metasfresh/issues/5237) Attribute "Herkunft" is not updated after country change
  * [#5238](https://github.com/metasfresh/metasfresh/issues/5238) Finetuning Area Search: Params from selected BPartner>>Location
  * [#5239](https://github.com/metasfresh/metasfresh/issues/5239) Jasper for Customs Invoice
  * [#5261](https://github.com/metasfresh/metasfresh/issues/5261) Prevent Users from Accidentally deleting attachment files
  * [#5262](https://github.com/metasfresh/metasfresh/issues/5262) Adjustments for Specifications
  * [#5265](https://github.com/metasfresh/metasfresh/issues/5265) Show different Bestellkontrolle views in Jasper based on type
  * [#5276](https://github.com/metasfresh/metasfresh/issues/5276) Finetuning dunning window
  * [#5282](https://github.com/metasfresh/metasfresh/issues/5282) WARN if webui.frontend.url is not configured
  * [#5285](https://github.com/metasfresh/metasfresh/issues/5285) Make sure AD_Column.IsTranslatable could be set when the column is eligible
  * [#5288](https://github.com/metasfresh/metasfresh/issues/5288) Customization tool: Process to add/update a field to selected UI element group
  * [#5290](https://github.com/metasfresh/metasfresh/issues/5290) Fix BPartner->Vendor wrong tab name
  * [#5291](https://github.com/metasfresh/metasfresh/issues/5291) Automated test: make sure RepoIds are correctly defined

* metasfresh-webui-frontend
  * [#2284](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2284) Make OpenViewAction open data in a new browser tab
  * [#2287](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2287) Add a confirmation popup before deleting attachment file

## Fixes

* metasfresh
  * [#5280](https://github.com/metasfresh/metasfresh/issues/5280) Enable MetasfreshIssueAppender when the system is ready for it
  * [#5284](https://github.com/metasfresh/metasfresh/issues/5284) Non-Barcode Order-Checkup doesn't show C_BPartner_Location.Name

* metasfresh-webui-api
  * [#1206](https://github.com/metasfresh/metasfresh-webui-api/issues/1206) HU Transform and Serial Number Processes don't start

* metasfresh-webui-frontend
  * [#2149](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2149) Decimal value .00 not added to product price at first
  * [#2232](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2232) Wrong Button color after first Date click in Range Widget
  * [#2274](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2274) Calendar icon should react to clicks
  * [#2279](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2279) Patching broken for Attributes widget

# metasfresh 5.106

## Features
* metasfresh
  * [#5205](https://github.com/metasfresh/metasfresh/issues/5205) Improve IFA import
  * [#5212](https://github.com/metasfresh/metasfresh/issues/5212) Add Specifications product report
  * [#5216](https://github.com/metasfresh/metasfresh/issues/5216) Allow deleting candidates if processed_override and not invoiced
  * [#5224](https://github.com/metasfresh/metasfresh/issues/5224) Adjust Balance report
  * [#5229](https://github.com/metasfresh/metasfresh/issues/5229) Adjust production order report

## Fixes
* metasfresh-e2e
  * [#87](https://github.com/metasfresh/metasfresh-e2e/issues/87) Filter buttons not reachable if many records
  * [#91](https://github.com/metasfresh/metasfresh-e2e/issues/91) Fix sales order to invoice test

# metasfresh 5.105

## Features
* metasfresh
  * [#5181](https://github.com/metasfresh/metasfresh/issues/5181) Add Age and Production Date attributes
  * [#5192](https://github.com/metasfresh/metasfresh/issues/5192) Add a less restrictive C_Postal Unique Index
  * [#5198](https://github.com/metasfresh/metasfresh/issues/5198) HU Mass Disposal process
  * [#5199](https://github.com/metasfresh/metasfresh/issues/5199) Avoid updating AD_EventLog records
  * [#5214](https://github.com/metasfresh/metasfresh/issues/5214) Change OLCand-Processor config to process OLCands from OrderLineCandidate REST EP

## Fixes
* metasfresh
  * [#5206](https://github.com/metasfresh/metasfresh/issues/5206) BPartnerGroup and Product UOM are not set automatically anymore in new bpartner / new product

* metasfresh-webui-frontend
  * [#2263](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2263) HU Panel too small in material receipt candidates' modal overlay
  * [#2265](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2265) Notifications and user menu will not close
  * [#2272](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2272) frontend fields readonly during (patch) request

# metasfresh 5.104

## Features
* metasfresh
  * [#5101](https://github.com/metasfresh/metasfresh/issues/5101) Area search - Geocoding
  * [#5175](https://github.com/metasfresh/metasfresh/issues/5175) Add language parameter to SQL Function PP_Product_BOM_Recursive
  * [#5177](https://github.com/metasfresh/metasfresh/issues/5177) Checking BtM and PZN with Modulo 11
  * [#5183](https://github.com/metasfresh/metasfresh/issues/5183) Enable selective cache invalidation

* metasfresh-e2e
  * [#74](https://github.com/metasfresh/metasfresh-e2e/issues/74) Create new Tax Rate
  * [#76](https://github.com/metasfresh/metasfresh-e2e/issues/76) Set currency USD active/inactive
  * [#78](https://github.com/metasfresh/metasfresh-e2e/issues/78) Enable checking for user notifications

## Fixes
* metasfresh
  * [#5172](https://github.com/metasfresh/metasfresh/issues/5172) Pricing Conditions Report Error
  * [#5182](https://github.com/metasfresh/metasfresh/issues/5182) forum-datenaustausch.ch XML externalId not sufficiently unique
  * [#5185](https://github.com/metasfresh/metasfresh/issues/5185) forum-datenaustausch.ch XML pre-existing documents are removed from XML on exporting
  * [#5186](https://github.com/metasfresh/metasfresh/issues/5186) Invoice candidate from order line candidate - pricelist precision not applied when computing PriceActual

* metasfresh-webui-api
  * [#1189](https://github.com/metasfresh/metasfresh-webui-api/issues/1189) Results missing in batch entry dropdown
  * [#1194](https://github.com/metasfresh/metasfresh-webui-api/issues/1194) Non-Mandatory BigDecimal fields inititalized with 0

* metasfresh-e2e
  * [#79](https://github.com/metasfresh/metasfresh-e2e/issues/79) Fix sales order test

# metasfresh 5.103
## Features
* metasfresh
  * [#5137](https://github.com/metasfresh/metasfresh/issues/5137) Inventory with multiple HUs per inventory line

## Fixes
* metasfresh-webui-api
  * [#1190](https://github.com/metasfresh/metasfresh-webui-api/issues/1190) HU received in manufacturing order cannot be selected for issueing in a second manufacturing order

* metasfresh-webui-frontend
  * [#2251](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2251) Attributes panel displayed only after blurring button

* metasfresh-e2e
  * [#19](https://github.com/metasfresh/metasfresh-e2e/issues/19) Fix Test purchase_create_vendor
  * [#37](https://github.com/metasfresh/metasfresh-e2e/issues/37) eslint delete CR error in project
  * [#39](https://github.com/metasfresh/metasfresh-e2e/issues/39) Use fixtures for attributes
  * [#57](https://github.com/metasfresh/metasfresh-e2e/issues/57) Fix bpartner object: location
  * [#58](https://github.com/metasfresh/metasfresh-e2e/issues/58) Fix isChecked command
  * [#66](https://github.com/metasfresh/metasfresh-e2e/issues/66) Fix Test: Sysconfig


# metasfresh 5.102
## Features
* metasfresh 
  * [#5151](https://github.com/metasfresh/metasfresh/issues/5151) Allow to delete Scale Prices
  * [#5157](https://github.com/metasfresh/metasfresh/issues/5157) Reduce log-output of sequence checks when running migration-script

* metasfresh-webui-frontend
  * [#2180](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2180) Shortcut shall work for Cancel button in Modal view
  * [#2195](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2195) Tab top actions: use provided shortcut if any

* metasfresh-e2e
  * [#53](https://github.com/metasfresh/metasfresh-e2e/issues/53) Add repeatable actions for working with filters

# metasfresh 5.101
## Features
* metasfresh
  * [#5108](https://github.com/metasfresh/metasfresh/issues/5108) Short term availability check for sales orders
  * [#5143](https://github.com/metasfresh/metasfresh/issues/5143) Product Specification process only for one selected product

* metasfresh-e2e
  * [#36](https://github.com/metasfresh/metasfresh-e2e/issues/36) Use fixtures for sales order

* metasfresh-edi
  * [#3](https://github.com/metasfresh/metasfresh-edi/issues/3) Process new data formats

## Fixes
* metasfresh-webui-frontend
  * [#2217](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2217) Console flooded with error "Cannot read property 'getInstance' of null"


# metasfresh 5.100
## Features
* metasfresh
  * [#5114](https://github.com/metasfresh/metasfresh/issues/5114) Column Translation Insert
  * [#5121](https://github.com/metasfresh/metasfresh/issues/5121) Create Company Directory window
  * [#5123](https://github.com/metasfresh/metasfresh/issues/5123) Don't automatically generate AD_Message records for developers
  * [#5131](https://github.com/metasfresh/metasfresh/issues/5131) SQL rollout: consider additional URLs to download and run the migation scripts


## Fixes
* metasfresh
  * [#5119](https://github.com/metasfresh/metasfresh/issues/5119) Fix AD_Element_Link related issues
  * [#5128](https://github.com/metasfresh/metasfresh/issues/5128) Avoid generating values for "Value" column when dealing with application dictionary entities
  * [#5134](https://github.com/metasfresh/metasfresh/issues/5134) Repair Umsatzreport Geschäftspartner Woche Excel

* metasfresh-webui-frontend
  * [#2241](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2241) Order line quick input not working
  * [#2244](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2244) Fix tabbing

# metasfresh 5.99
## Features
* metasfresh
  * [#5024](https://github.com/metasfresh/metasfresh/issues/5024) REST API for sales invoice payment status
  * [#5095](https://github.com/metasfresh/metasfresh/issues/5095) Enable set/unset of BPartner narcotics pharma permission
  * [#5118](https://github.com/metasfresh/metasfresh/issues/5118) Tool to run all migration scripts from developer workspace

* metasfresh-e2e
  * [#16](https://github.com/metasfresh/metasfresh-e2e/issues/16) Make our custom input commands more stable

# Fixes
* metasfresh-webui-frontend
  * [#2214](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2214) Input field value sometimes swallowed
  * [#2237](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2237) Scrollbars missing in modal overlays

# metasfresh 5.98
## Features
* metasfresh 
  * [#4895](https://github.com/metasfresh/metasfresh/issues/4895) Support Automatic Numbering on Purchase Requisition
  * [#4951](https://github.com/metasfresh/metasfresh/issues/4951) Phonecall Planning and Execution
  * [#5040](https://github.com/metasfresh/metasfresh/issues/5040) Accounting for Payment Allocation and Vendor Credit Memo wrong
  * [#5070](https://github.com/metasfresh/metasfresh/issues/5070) Discount Schema Lines in separate window
  * [#5072](https://github.com/metasfresh/metasfresh/issues/5072) Support forum-datenaustausch.ch XML invoice cancelation-response
  * [#5081](https://github.com/metasfresh/metasfresh/issues/5081) Product prices window: don't sort it because on huge amount of data this is a performance issue
  * [#5089](https://github.com/metasfresh/metasfresh/issues/5089) XML import/export for Kanton 

* metasfresh-webui-api
  * [#1178](https://github.com/metasfresh/metasfresh-webui-api/issues/1178) view: kick out a row if is no longer matching the filters

* metasfresh-webui-frontend
  * [#2221](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2221) Display time fields with no seconds in gridview
  * [#2224](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2224) View: after calling getByIds, frontend shall remove the rows which are no longer in the result

* metasfresh-edi
  * [#1](https://github.com/metasfresh/metasfresh-edi/issues/1) Modernize and update EDI ESB camel

# Fixes
* metasfresh
  * [#5079](https://github.com/metasfresh/metasfresh/issues/5079) Error while posting purchase invoices because of charge even though charge is not used
  * [#5084](https://github.com/metasfresh/metasfresh/issues/5084) Error while posting cost collector
  * [#5086](https://github.com/metasfresh/metasfresh/issues/5086) Error logging in to webui when there is no default warehouse
  * [#5092](https://github.com/metasfresh/metasfresh/issues/5092) Fix wrong avg PO cost on material receipt and match invoice in case we have a different price UOM
  * [#5093](https://github.com/metasfresh/metasfresh/issues/5053) Log related NPE on metasfresh startup

* metasfresh-webui-api
  * [#1180](https://github.com/metasfresh/metasfresh-webui-api/issues/1180) Webui server shall start even if something in picking terminal code fails

* metasfresh-webui-frontend
  * [#2230](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2230) Refresh filtered list

# metasfresh 5.97
## Features
* metasfresh
  * [#5051](https://github.com/metasfresh/metasfresh/issues/5051) Allow the formatting of IBAN in BPartner Bank
  * [#5068](https://github.com/metasfresh/metasfresh/issues/5068) Dataentry Implementation Fieldname larger
  * [#5059](https://github.com/metasfresh/metasfresh/issues/5059) DataEntry - change terminology

* metasfresh-webui-api
  * [#1175](https://github.com/metasfresh/metasfresh-webui-api/issues/1174) Provide View Header Properties to be displayed on frontend

* metasfresh-webui-frontend
  * [#2209](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2209) Single entry changes
  * [#2220](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2220) More changes to data entry tab

## Fixes
* metasfresh
  * [#5028](https://github.com/metasfresh/metasfresh/issues/5028) Order candidate - missing SyncAdvise for Org on-the-fly-creation/update
  * [#5048](https://github.com/metasfresh/metasfresh/issues/5048) Average purchase cost is updating the Price as per the Price Unit and not as per the Items Base UoM
  * [#5053](https://github.com/metasfresh/metasfresh/issues/5053) Log related NPE on metasfresh startup
  * [#5055](https://github.com/metasfresh/metasfresh/issues/5055) IFA fields shall be Readonly in Pharma Product window
  * [#5061](https://github.com/metasfresh/metasfresh/issues/5061) Deadlock in CConnection.get() when the metasfresh.properties is not already created

* metasfresh-webui-api
  * [#1175](https://github.com/metasfresh/metasfresh-webui-api/issues/1175) Picking v2: Products to pick view shall show order no, customer name and preparation time in header
  * [#1177](https://github.com/metasfresh/metasfresh-webui-api/issues/1177) Error on order quick entry

# metasfresh 5.96
## Features
* metasfresh
  * [#4959](https://github.com/metasfresh/metasfresh/issues/4959) Data entry implementation

* metasfresh-webui-api
  * [#1165](https://github.com/metasfresh/metasfresh-webui-api/issues/1165) Window Layout: allow first field of a fields combo to be a dropdown
  * [#1167](https://github.com/metasfresh/metasfresh-webui-api/issues/1167) Product lookup performance improvements (repsective frontend isue not yet done)

* metasfresh-webui-frontend
  * [#2177](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2177) Support single entry view mode for Tabs

## Fixes
* metasfresh-webui-api
  * [#1163](https://github.com/metasfresh/metasfresh-webui-api/issues/1163) Warehouse cannot be created / opening window causes error

* metasfresh-webui-frontend
  * [#2201](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2201) Attributes panel is not displayed in HU Editor
  * [#2204](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2204) QR Code not displayed


# metasfresh 5.95
# Features
* metasfresh
  * [#5012](https://github.com/metasfresh/metasfresh/issues/5012) Add Cable Batchentry also to Purchase Order
  * [#5014](https://github.com/metasfresh/metasfresh/issues/5014) Make SQL Statement column larger in Report and Process
  * [#5021](https://github.com/metasfresh/metasfresh/issues/5021) Allow deleting AD_Tabs
  * [#5026](https://github.com/metasfresh/metasfresh/issues/5026) XJC timeout on reading XSDs
  * [#5030](https://github.com/metasfresh/metasfresh/issues/5030) Migration scripts applier: run after scripts executed database function

# Fixes
* metasfresh
  * [#4999](https://github.com/metasfresh/metasfresh/issues/4999) Packed HUs not displayed as Picked in HU Editor
  * [#5000](https://github.com/metasfresh/metasfresh/issues/5000) Not all invoice candidates are invoiced with Process action in Picking Terminal v2

* metasfresh-webui-frontend
  * [#2199](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2199) Fix sending tab data when creating process modal

# metasfresh 5.94
# Features
* metasfresh
  * [#4913](https://github.com/metasfresh/metasfresh/issues/4913) Add payment discount when importing discount schema
  * [#4961](https://github.com/metasfresh/metasfresh/issues/4961) Chart of Accounts Import
  * [#4982](https://github.com/metasfresh/metasfresh/issues/4982) AD_Element_Trl customization
  * [#4988](https://github.com/metasfresh/metasfresh/issues/4988) Improve async workpackage logging for shipment schedule and invoice candidate updating
  * [#4991](https://github.com/metasfresh/metasfresh/issues/4991) URL csv Importer for BPartner
  * [#4997](https://github.com/metasfresh/metasfresh/issues/4997) Handle M_DiscountSchemaBreak with PriceBase=P(ricingSystem) & missing Base_PricingSystem_ID
  * [#5001](https://github.com/metasfresh/metasfresh/issues/5001) Create a table for storing product certificate informations

* metasfresh-webui
  * [#1945](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1945) "About" action in webui

* metasfresh-webui-frontend
  * [#2197](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2197) Don't show input field for QR reader on mobile

# Fixes
* metasfresh
  * [#4966](https://github.com/metasfresh/metasfresh/issues/4966) Prolonging contract does not working anymore
  * [#4975](https://github.com/metasfresh/metasfresh/issues/4975) LastShipmentDate not displayed anymore in Products Proposal
  * [#4985](https://github.com/metasfresh/metasfresh/issues/4985) MemorizingSupplier.get returns null while it actually couldn't
  * [#4987](https://github.com/metasfresh/metasfresh/issues/4987) M_Attribute_Value is not saved correctly
  * [#4989](https://github.com/metasfresh/metasfresh/issues/4989) Problem posting documents with zero-amounts

# metasfresh 5.93
# Features
* metasfresh
  * [#4967](https://github.com/metasfresh/metasfresh/issues/4967) Warehouse Customization: Picking

* metasfresh-webui-api
  * [#1154](https://github.com/metasfresh/metasfresh-webui-api/issues/1154) Take out "Back" action from quick actions in "More products..." modal
  * [#1155](https://github.com/metasfresh/metasfresh-webui-api/issues/1155) Support providing shortcuts for processes

* metasfresh-webui-frontend 
  * [#2182](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2182) Back button for modals
  * [#2183](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2183) frontend: Scan using camera shall be translatable
  * [#2193](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2193) View quick actions: provide viewProfileId when calling /quickActions endpoint

# Fixes
* metasfresh
  * [#4964](https://github.com/metasfresh/metasfresh/issues/4964) Services.get(IDocumentNoBuilderFactory.class) calls the wrong constructor
  * [#4976](https://github.com/metasfresh/metasfresh/issues/4976) M_DiscountSchemaBreak.PriceBase shall be nullable

* metasfresh-dist
  * [#57](https://github.com/metasfresh/metasfresh-dist/issues/57) PostgreSQL applying our migration scripts not working anymore

# metasfresh 5.92
# Features
* metasfresh
  * [#4916](https://github.com/metasfresh/metasfresh/issues/4916) Checkbox Newsletter in der Neuaufnahme anzeigen
  * [#4952](https://github.com/metasfresh/metasfresh/issues/4952) Implement Campain Pricing Rule
  * [#4953](https://github.com/metasfresh/metasfresh/issues/4953) Add taxId to function docs_generics_org_report

* metasfresh-webui-api
  * [#1142](https://github.com/metasfresh/metasfresh-webui-api/issues/1142) Make Issue CUs from Source HU work for Multi Select
  * [#1148](https://github.com/metasfresh/metasfresh-webui-api/issues/1148) Products proposal: display the prices paid by other customers

* metasfresh-webui-frontend
  * [#2147](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2147) Display process descriptions that are provided by the API
  * [#2157](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2157) frontend: Document included tab: pluggable actions to start a process

# Fix
* metasfresh-webui-frontend
  * [#2145](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2145) Model view: row no longer refreshed
  * [#2160](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2160) Selected row not always correctly recognized
  * [#2162](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2162) View quick actions shall not display scrollbar

# metasfresh 5.91
# Features
* metasfresh
  * [#4941](https://github.com/metasfresh/metasfresh/issues/4941) Add option to not translate words that exist as elements or messages
  * [#4935](https://github.com/metasfresh/metasfresh/issues/4935) Create MTransaction when completing cost collector of type issue/receipt
  * [#4936](https://github.com/metasfresh/metasfresh/issues/4936) Use latest c3p0 and postgres driver

* metasfresh-webui-frontend
  * [#2158](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2158) Modal view: Cancel button support
  * [#2169](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2169) Host google fonts locally

# metasfresh 5.90
# Features
* metasfresh
  * [#4894](https://github.com/metasfresh/metasfresh/issues/4894) BPartner Product statistics: LastShipmentDate, LastReceiptDate
  * [#4903](https://github.com/metasfresh/metasfresh/issues/4903) Introduce AD_Table_Process.AD_Table_Process_ID primary key
  * [#4906](https://github.com/metasfresh/metasfresh/issues/4906) Pricing: fallback to base price list version if any
  * [#4911](https://github.com/metasfresh/metasfresh/issues/4911) Translate the C_BPartner label fields to German
  * [#4915](https://github.com/metasfresh/metasfresh/issues/4915) Improve error handling when ID server is not correctly configured

* metasfresh-webui-api
  * [#1134](https://github.com/metasfresh/metasfresh-webui-api/issues/1134) Document included tab: provide actions to be displayed in included tab's top lane


# metasfresh 5.89
# Features
* metasfresh
  * [#4881](https://github.com/metasfresh/metasfresh/issues/4881) Different improvements around MSV3 server synchronization
  * [#4883](https://github.com/metasfresh/metasfresh/issues/4883) Quickactions in Invoice Candidates Window
  * [#4886](https://github.com/metasfresh/metasfresh/issues/4886) Account Schema window: don't allow creating new accounting schemas
  * [#4887](https://github.com/metasfresh/metasfresh/issues/4887) New Window Tab: callout to automatically set AD_Element_ID, Name, InternalName when a table is selected
  * [#4892](https://github.com/metasfresh/metasfresh/issues/4892) Add inactive product fields for hu tracing and label printing
  * [#4894](https://github.com/metasfresh/metasfresh/issues/4894) BPartner Product statistics: LastShipmentDate, LastReceiptDate


* metasfresh-webui-api
  * [#1128](https://github.com/metasfresh/metasfresh-webui-api/issues/1128) Limit number of products shown in material cockpit
  * [#1132](https://github.com/metasfresh/metasfresh-webui-api/issues/1132) Sales/Purchase order: customer proposal products list
  * [#1130](https://github.com/metasfresh/metasfresh-webui-api/issues/1130) Restrict DocumentCollection cache size

# Fixes
* metasfresh
  * [#4896](https://github.com/metasfresh/metasfresh/issues/4896) Errors in Tax Codes Report
  * [#4900](https://github.com/metasfresh/metasfresh/issues/4900) AD_Val_Rule ESR_Import_AD_AttachmentEntry is broken
  * [#4902](https://github.com/metasfresh/metasfresh/issues/4902) Process BPartnerOrgLink doesn't set AD_OrgInfo.OrgBP_Location_ID


# metasfresh 5.88
# Features
* metasfresh 
  * [#4866](https://github.com/metasfresh/metasfresh/issues/4866) Create purchase orders: if the vendor is using a gateway then always order directly
  * [#4868](https://github.com/metasfresh/metasfresh/issues/4868) Make C_PurchaseCandidate.IsAggregatePO a searchable column

# Fixes
* metasfresh
  * [#4782](https://github.com/metasfresh/metasfresh/issues/4782) Various fixes to import processes
  * [#4859](https://github.com/metasfresh/metasfresh/issues/4859) Durchschnittspreise SQL ergibt Fehlerhafte Daten (Preis Abw. nicht berücksichtigt)
  * [#4876](https://github.com/metasfresh/metasfresh/issues/4876) Inventory related fixes
  * [#4873](https://github.com/metasfresh/metasfresh/issues/4873) Product: The Temperature Field is too short

* metasfresh-webui-api
  * [#1123](https://github.com/metasfresh/metasfresh-webui-api/issues/1123) Fix process parameter translations
  * [#1125](https://github.com/metasfresh/metasfresh-webui-api/issues/1125) Fix webui window update from remote editing
  * [#1127](https://github.com/metasfresh/metasfresh-webui-api/issues/1127) Cache invalidation failing - null childLinkColumnName

* metasfresh-webui-frontend
  * [#2148](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2148) Tables not fully displayed in windows causing filters and actions not being displayed properly

# metasfresh 5.87
# Features
* metasfresh
  * [#4798](https://github.com/metasfresh/metasfresh/issues/4798) AD_RefList Description shall be shown in webui
  * [#4863](https://github.com/metasfresh/metasfresh/issues/4863) Add created/ updated to asynch workpackage and filter for created
  * [#4857](https://github.com/metasfresh/metasfresh/issues/4857) Add PK column AD_OrgInfo_ID

* metasfresh-webui-api
  * [#1119](https://github.com/metasfresh/metasfresh-webui-api/issues/1119) Max rows loaded in a included tab shall be configurable

# Fixes
* metasfresh 
  * [#4862](https://github.com/metasfresh/metasfresh/issues/4862) When deleting a AD_Tab, the AD_Field and AD_Element_Link records shall be deleted

* metasfresh-webui-frontend
  * [#2119](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2119) Screen turns grey for 1 sec sometimes
  * [#2120](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2120) Tab not always working correctly
  * [#2122](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2122) Quick actions dropdown covered by pagination in modals
  * [#2124](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2124) Webcam Foto not working anymore since last chrome update
  * [#2130](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2130) Header/subheader not working correctly on mobile
  * [#2133](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2133) Display value description when hovering over field
  * [#2135](https://github.com/metasfresh/metasfresh-webui-frontend/pull/2135) Sync all contract specs - add contracted vendor and discount schema
  * [#2034](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2034) Uncaught TypeError: selected.indexOf is not a function
  * [#2134](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2134) string field is reset in mid-typing
  * [#2148](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2148) Tables not fully displayed in windows causing filters and actions not being displayed properly

# metasfresh 5.86
# Features
* metasfresh
  * [#4310](https://github.com/metasfresh/metasfresh/issues/4310) WebUI: add Manufacturer field in Pricing Conditions
  * [#4820](https://github.com/metasfresh/metasfresh/issues/4820) Categorize Business Partners as "Neukunde", "Stammkunde"
  * [#4840](https://github.com/metasfresh/metasfresh/pull/4840) ITableRefInfo - rename "name" to "identifier" and make it more verbose
  * [#4842](https://github.com/metasfresh/metasfresh/issues/4842) Implement Excel Open XML format support
  * [#4848](https://github.com/metasfresh/metasfresh/issues/4848) mass-invoicing improvements

# Fixes
* metasfresh
  * [#4843](https://github.com/metasfresh/metasfresh/issues/4843) InterfaceWrapperHelper.newInstance(I_AD_OrgInfo.class) returns null
  * [#4846](https://github.com/metasfresh/metasfresh/issues/4846) Contract extension does not set date correctly

* metasfresh-webui-api
  * [#968](https://github.com/metasfresh/metasfresh-webui-api/issues/968) Error msg missing when trying to create flatrate term from bpartner window in case of no bpartner location
  * [#1113](https://github.com/metasfresh/metasfresh-webui-api/issues/1113) Generate PO from Sales order not working anymore

* metasfresh-webui-frontend
  * [#2075](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2075) Deselecting lines does not work when clicking everywhere outside of table
    * Improvement of the deselection Handling of Grid Table Rows. Now it's possible to deseclect by clicking any areas outside table.
  * [#2104](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2104) Show error msg when pricelist is not saved bc of UQ index missing for InternalName and Price system in Price list
    * Shows an error now, when Pricelist Name is not unique.
  * [#2111](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2111) Additional Dropdown in menu search in latest Chrome
    * Removes the Google Chrome Search result proposal.
  * [#2112](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2112) Overlays open in narrow window on latest Chrome
  * [#2116](https://github.com/metasfresh/metasfresh-webui-frontend/pull/2116) Fix specs in cypress/integration/contracts
  * [#2117](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2117) Barcode scanner looks bad in filters
    * Improvement of the Barcode Scanner Look&Feel in Filter Menu entry.
  * [#2128](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2128) View: select all no longer works

* metasfresh-dist
  * [#55](https://github.com/metasfresh/metasfresh-dist/pull/55) introduce a parameter to set the DB seed's URL

# metasfresh 5.85
# Features
* metasfresh
  * [#4809](https://github.com/metasfresh/metasfresh/pull/4809) Make contact persons's location editable under circumstances
    * Improving the behavior when editing the location of contact persons in some minor cases.
  * [#4823](https://github.com/metasfresh/metasfresh/issues/4823) CSV import BP URL
    * Extended Business Partner import, now allowing to import the Businesspartner Website URL aswell.
  * [#4825](https://github.com/metasfresh/metasfresh/issues/4825) invoice and async improvements
    * Improvement of logging for skipped asynch Work Packages.
  * [#4828](https://github.com/metasfresh/metasfresh/issues/4828) Extend OLCand REST API to allow not to create products on the fly
    * Extended Functionality in Orderlines Candidates REST-API.
  * [#4832](https://github.com/metasfresh/metasfresh/issues/4832) Extend Datenaustausch-Config and XML modding
    * Extending the Format of forum-datenaustusche Datenaustausch Configuration and bahavior
  * [#4837](https://github.com/metasfresh/metasfresh/issues/4837) Add fiscal year 2019 to our standard calendar
    * Adding the fiscal year 2019 to the default accounting calendar.

* metasfresh-webui-frontend
  * [#2097](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2097) Lookup and Dropdown: Empty list entry for non mandatory
    * New Feature, now steering the mandatory Logic of List and Lookup widgets in WebUI.
  * [#2098](https://github.com/metasfresh/metasfresh-webui-frontend/pull/2098) extract the edit-location code into a command
    * Extracting the edit location into a cypress command, to make it reusable for other tests.

# Fixes
* metasfresh
  * [#4679](https://github.com/metasfresh/metasfresh/issues/4679) Solve print info UI performance problem
    * Improves thje Performance in WebUI for Print Info.
  * [#4805](https://github.com/metasfresh/metasfresh/issues/4805) ATP not correct after partial material receipt
    * Fixes the Available to Promise calculation after doing partial Material Receipt.
  * [#4827](https://github.com/metasfresh/metasfresh/issues/4827) Forward C_OLCand POReference to C_Invoice_Candidate
    * Bugfix for the PO Reference fowarding from Order Candidates to invoice Candidates.
  * [#4829](https://github.com/metasfresh/metasfresh/issues/4829) Add Unique index for InternalName and Price system in Price list
    * Internal improvement of Price List, adding a unique index for internal name and price system.

* metasfresh-webui-api
  * [#1114](https://github.com/metasfresh/metasfresh-webui-api/issues/1114) webui frontend does nothing in latest chrome

* metasfresh-webui-frontend
  * [#1253](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1253) Problem with composed fields with non-mandatory elements
    * Adds None Option to Lookup widget dropdowns, that alows o overwrite already set a selection in a non mandatory field.
  * [#2047](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2047) Run QR code action: sometimes ESC does not work
    * Improves the handling of escape shortcut in QR Code action.
  * [#2103](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2103) Chrome feature overwrites country selection in Lookup
    * Fixes the behavior of WebUI after some changes in the latest Chrome update.
  * [#2109](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2109) Chrome not recognized properly
    * Fixes the behavior of WebUI after some changes in the latest Chrome update.
  
# metasfresh 5.84
# Features
* metasfresh-webui-frontend
  * [#2077](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2077) Make references cypress friendly
    * Now returning the internal name via API to make references more cypress friendly.
  * [#2080](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2080) Support to create C_Location via cypress
    * Improvement that allows to creates Locations via Cypress Tests.
  * [#2082](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2082) Show tab description as tool tip
    * New Feature that now shows Tab Descriptions as tooltip when hovering.
  * [#2086](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2086) Individual Logo shall not have hashsequence added to name
    * Removes the hash sequence from individual Logo Name, now allowing to replace the metasfresh Logo automatically via CI Build.
  * [#2090](https://github.com/metasfresh/metasfresh-webui-frontend/pull/2090) Update to Node.js 11
    * Updates frontend to Node.js 11.

# Fixes
* metasfresh
  * [#4811](https://github.com/metasfresh/metasfresh/issues/4811) Price using BOM Line's attribute is not calculated correctly
    * Fixes the new BOM Component Attribute Price calculation.
  * [#4819](https://github.com/metasfresh/metasfresh/issues/4819) Payment allocation posting error for currency gain/loss and discount/writeoff case
    * Bugfix for the posting of Payment Allocation cornercase with currency gain/ loss involved.
  * [#4821](https://github.com/metasfresh/metasfresh/issues/4821) forum-datenaustausch.ch export XML validation errors
    * Fixes the forum-datenaustuasch.ch validation errors.

* metasfresh-webui-frontend
  * [#2064](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2064) Warning: Failed prop type: Invalid prop `logged` of type `string` supplied to `Login`, expected `boolean`
    * Fixes a console error that appeared when redirecting to another window via link directly through login.
  * [#2066](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2066) Changes in tabs in grid view not always patched (e.g. description in orderline)
    * Improves the behavior of Text changing confirmation.
  * [#2070](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2070) Number changing in order line grid view
    * Improves the behavior of Number changing confirmation.
  * [#2086](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2086) Individual Logo shall not have hashsequence added to name
    * Improves the Logo Handling in Build process. Now not adding a hash anymore to the logo file, which makes it easier to automate individual logos in Build process.

# metasfresh 5.83
# Features
* metasfresh
  * [#4787](https://github.com/metasfresh/metasfresh/issues/4787) Product Document Note Translation
    * New Feature that allows to translate the Document Notes.
  * [#4789](https://github.com/metasfresh/metasfresh/issues/4789) C_BPartner filter for IsActive
    * New Filter in Business Partner window that allowes to show only active Business Partners.
  * [#4795](https://github.com/metasfresh/metasfresh/issues/4795) Product No. of customer also with ASI
    * New Feature that makes it possible to define customer Product No. based on Attribute values.

* metasfresh-webui-api
  * [#1111](https://github.com/metasfresh/metasfresh-webui-api/issues/1111) Include internalName in JSONReference
    * Now the internal Name is delivered by API which can be used in Cpress Tests.

* metasfresh-webui-frontend
  * [#2083](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2083) Cypress pressDoneButton shall fail if the respective record was not saved
    * Cypress Test that fails if the record was not saved yet when pressing the Done button.

# Fixes
* metasfresh
  * [#4793](https://github.com/metasfresh/metasfresh/issues/4793) View docs_sales_invoice_details_compensation_subgroup: the invoice detail shall be taken from invoice
    * Adjustment of Jasper Invoice Document, now taking further invoice details from invoiceline, instead of orderline.
  * [#4797](https://github.com/metasfresh/metasfresh/issues/4797) HU Trace window: filtering by HUTaceType returns no results
    * Fixes the filtering in Handling Unit Trace Window, now able to filter the HU Trace Type again.
  * [#4802](https://github.com/metasfresh/metasfresh/issues/4802) Required IfExists parameter 'ifBPartnersExist' is not present
    * Internal fix for Fix for 'ifBPartnersExist' parm.

* metasfresh-webui-frontend
  * [#2073](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2073) Failing cypress tests
    * Fixes some failing Cypress Tests.

# metasfresh 5.82
# Features
* metasfresh
  * [#4662](https://github.com/metasfresh/metasfresh/issues/4662) AD_Element based Names and Translations for AD_Tab, Window, Menu
    * New and easier Translation Functionality for Tab, Window and Manu Elements.
  * [#4663](https://github.com/metasfresh/metasfresh/issues/4663) Add base language to AD_Element Translation Tables
    * The Base Language of the System is now stored on Element Level too making it much easier to maintain.
  * [#4664](https://github.com/metasfresh/metasfresh/issues/4664) New Window "Application Elements"
    * New Window in WebUI that Allows to maintain the Window Element Names and Description in a central place.
  * [#4717](https://github.com/metasfresh/metasfresh/issues/4717) Set Order-Checkup printout receiver via AD_Workflow
    * Improvement of the Printing Routing. Now receiving printing Information for Manufacturing via workflows, instead of warehouse.
  * [#4737](https://github.com/metasfresh/metasfresh/issues/4737) Fix attribute value lookup for webui
    * Minor Improvement of the Attribute value Lookup in WebUI.
  * [#4745](https://github.com/metasfresh/metasfresh/issues/4745) Allow editing attachment descriptions in BPartner-B2C
    * Feature to Edit attachment descriptions in Businesspartner B2C window in WebUI.
  * [#4756](https://github.com/metasfresh/metasfresh/issues/4756) order-candidates REST-API - option to just lookup, but not create BPartners
    * New Endpoint in Rest API to lookup Business Partners.
  * [#4763](https://github.com/metasfresh/metasfresh/issues/4763) Update material dispo correction from StockChangedEvents
    * Improvement of the Material Disposition. Now updateing adjustment from Stock Change Events.
  * [#4764](https://github.com/metasfresh/metasfresh/issues/4764) Translation of Greetings in WebUI
    * New Window for Greetings Translation in WebUI.
  * [#4766](https://github.com/metasfresh/metasfresh/issues/4766) C_OrderLine: ProductDescription - don't add qty from BOM if is one
    * Adjustment of the Orderline Product Description. Not adding the Quantity of 1 Unit in Product description anymore.
  * [#4768](https://github.com/metasfresh/metasfresh/issues/4768) ModelAttributeSetInstanceListener for Expired attribute
    * Improves the way, the expired Attribute is set.
  * [#4770](https://github.com/metasfresh/metasfresh/issues/4770) Improve ClasspathAnnotatedModelInterceptorTester
    * Internal housekeeping issue.
  * [#4771](https://github.com/metasfresh/metasfresh/issues/4771) Fix Fresh_AvailableSingletonServices_Test
    * Internal housekeeping issue.
  * [#4777](https://github.com/metasfresh/metasfresh/issues/4777) Import Address GLN via I_BPartner
    * Extends the Business Partner Import, now allowing to import GLN Information too.

# Fixes
* metasfresh
  * [#4740](https://github.com/metasfresh/metasfresh/issues/4740) Swing: "IOException: PDF header signature not found." for invoice print / print preview
    * Bugfix for Printing on metasfresh Swing Client that occurred when using the invoice print and print preview.
  * [#4754](https://github.com/metasfresh/metasfresh/issues/4754) Address different stability issues
    * Fixes different stability issues, mostly discovered in material receipt.
  * [#4759](https://github.com/metasfresh/metasfresh/issues/4759) Contract Condition Option No Invoice does not prevent Invoicing
    * Fixes the Configuration of No Invoice in Contracts, now not creating invoices when this option is set.
  * [#4773](https://github.com/metasfresh/metasfresh/issues/4773) google Reflections not working with maven surefire plugin
    * Internal Bugfix for using google reflections with the maven surefire plugin.
  * [#4775](https://github.com/metasfresh/metasfresh/issues/4775) Package order line out of sync when order is reactivated and completed again
    * Fixes a Bug in Orderline that occurred with out of sync package material lines after reactivating an Order.
  * [#4778](https://github.com/metasfresh/metasfresh/issues/4778) Fix failing tests when running de.metas.fresh all tests suite in eclipse
    * Fixes some failing automated tests.
  * [#4779](https://github.com/metasfresh/metasfresh/issues/4779) MD_Stock_Reset process includes planned HUs
    * Removes the Stock calulation for Handling Units with Status planned.

* metasfresh-webui-api
  * [#1108](https://github.com/metasfresh/metasfresh-webui-api/issues/1108) Migration Script Endpoint Improvement
    * Fixes a Bug in the Migration Script Endpoint

* metasfresh-webui-frontend
  * [#1997](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1997) Cypress: Product set Documentnote Test fails
    * Fixes the cypress test on setting Document Notes.
  * [#2048](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2048) View: clicking outside of table does not unselect the current selected lines
    * Bugfix for the unselecting of grid selections when clicking outside grid.
  * [#2058](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2058) Cannot close the HU Editor in manufacturing order anymore
    * Fixes a bug in modal Handling Unit Editor that prevented the unselecting of rows.
  * [#2067](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2067) Dropdown in bpartner field in order sometimes remains displayed after selecting bpartner
    * Fixes a minor Bug that occurred when selecting dropdown entries with mouse. Now closing the dropdown after selecting again.
  * [#2069](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2069) Number Inserting in Order Quick Input
    * Fixes the Batch Entry in Sales Order, now reacting creating a new line after pressing enter again.

* metasfresh-parent
  * [#25](https://github.com/metasfresh/metasfresh-parent/issues/25) jasper reports are compiled with wrong version
    * Fixes the Build Process in jenkins for the compilation of Jasper Reports. Now using the correct Jasper Version.

# metasfresh 5.81
## Features

* metasfresh
  * [#4734](https://github.com/metasfresh/metasfresh/issues/4734) Shipper transportation identifier shall contain documentNo, date and the shipper name
    * Improvement of the shipper transportation identifiere, now including the documentNo, date and shipper name.

* metasfresh-webui-frontend
  * [#2006](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2006) View selection for touch screens
    * Enhancement of selection behavior, now possible for touch screens to select and unselect rows with finger tap.

## Fixes
* metasfresh
  * [#4738](https://github.com/metasfresh/metasfresh/issues/4738) Error creating receipt schedule if order line was created via "add new"
    * Bugfix for the receiept schedule in case the orderline was created via add new button.
  * [#4739](https://github.com/metasfresh/metasfresh/issues/4739) Fix context parse errors while using order's product batch entry
    * Fixes product search and add new on orderline for Batch entry.
  * [#4741](https://github.com/metasfresh/metasfresh/issues/4741) Process C_Order_VoidWithRelatedDocsAndRecreate hangs
    * Improvement of Order voiding, now reverting the document and related documents too.
  * [#4742](https://github.com/metasfresh/metasfresh/issues/4742) Attachment-Download from BPartner B2C window broken
    * Fixes the download of Attachments from the B2C Business Partner window.
  * [#4743](https://github.com/metasfresh/metasfresh/issues/4743) C_Invoice_CreateExportData async WP processor runs into error with most "normal" invoices
    * Fixes a Bug that occurred when an Organisation Business Partner does not have a remit-to address nor an ESR account.

* metasfresh-webui-api
  * [#1097](https://github.com/metasfresh/metasfresh-webui-api/issues/1097) "Issue only for what was received" method: Issued HUs remain issued and don't get destroyed
    * Fixes the "Issue only for what was received" Method in manufacturing receipt.
  * [#1098](https://github.com/metasfresh/metasfresh-webui-api/issues/1098) Label Element filters not working
    * Fixes the Filtering of Label Elements/ Attributes.
  * [#1099](https://github.com/metasfresh/metasfresh-webui-api/issues/1099) Zooming into a parent column from a translation window not working
    * Improves the zoom To into the parent column from translation windows.
  * [#1102](https://github.com/metasfresh/metasfresh-webui-api/issues/1102) Document filters: consider empty strings as no filters
    * Empty Strings are now considered as a non set filter criteria.

* metasfresh-webui-frontend
  * [#2008](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2008) Business partner field in order: bpartner and location not alligned
    * Minor frontend Fix for Businesspartner Lookup widget dropdown alignment.
  * [#2012](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2012) Modal view's title is not set when opened from process
    * Improvement of modal overlays, now setting the overlay Title correctly when opened via process.
  * [#2015](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2015) Make sure `Run QR code action` process can be executed from everywhere
    * Fixes the QR Code action, so that it can be run from any window.
  * [#2029](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2029) View quickActions timing issue
    * Fixes a timing issue with Quick Actions in WebUI.
  * [#2039](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2039) Uncaught TypeError: e.toISO is not a function
    * Bugfix for an error in action "create purchase orders".
  * [#2049](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2049) quick actions: not refreshed on selection changed in tablet/mobile mode
    * Improvement of the Quickaction refreshing in case of changes selections.
  * [#2050](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2050) Views: refresh `quickActions` after `GET /byIds` shall consider current selected rows
    * Bugfix for the Quickactions in WebUI now considering the selected rows again.
  * [#2054](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2054) Error while trying to add a new sales order line using batch entry
    * Fixes the Batch entry in Sales Order.
  * [#2060](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2060) Text widgets are not PATCHED anymore
    * Fixes tha patching of Text widgets. Now these are patched again after change.
  * [#2061](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2061) Cannot untick filter checkbox
    * Fixes the Filter checkboxes, now it's possible to untick them again.

# metasfresh 5.80
## Features
* metasfresh
  * [#4690](https://github.com/metasfresh/metasfresh/issues/4690) Picking Terminal v2: filtering options
    * Improved Filterting Options now available in the new Picking Terminal.
  * [#4691](https://github.com/metasfresh/metasfresh/issues/4691) Picking Terminal v2: if there is not enough Qty in storage create a new Products To Pick line
    * New Handling Unit line shown in new Picking Terminal, in case the initial Handling Unit does not have enough quantity.
  * [#4703](https://github.com/metasfresh/metasfresh/issues/4703) Support forum-datenaustausch.ch XML dunning
    * Support for the swiss helthcare data exchange format of forum-datenaustausch.ch for dunning documents.
  * [#4705](https://github.com/metasfresh/metasfresh/issues/4705) Avoid SQL N+1 in HU source queries
    * Performance Improvement for generated SQL Queries in metasfresh backend. Initially popped up during Handling Unit queries performance issues.
  * [#4708](https://github.com/metasfresh/metasfresh/issues/4708) webui: Change my password does not work
    * Fix for the "change my password" functionality.
  * [#4719](https://github.com/metasfresh/metasfresh/issues/4719) Allow AD_Val_Rule to be auto-applied on new record
    * Application Dictionary Improvement, now allowing Validation Rules to be automatically applied for initial values of a record.

* metasfresh-webui-api
  * [#1094](https://github.com/metasfresh/metasfresh-webui-api/issues/1094) Login: Show a user friendly error when user or password is empty
    * Improvement of the Login workflow, now showing a user friendly info when the password is left empty.

## Fixes
* metasfresh
  * [#4732](https://github.com/metasfresh/metasfresh/issues/4732) Can not create a new order line using 'Add new'
    * Bugfix for the Add new Line Functionality in Sales and Purchase Order window.

* metasfresh-webui-api
  * [#1082](https://github.com/metasfresh/metasfresh-webui-api/issues/1082) Picking from source HU not working
    * Fixes a Bug in Picking workflow, now able to pick from Source Handling Units again.
  * [#1083](https://github.com/metasfresh/metasfresh-webui-api/issues/1083) QtyPicked in first window picking terminal not correct
    * Improvement of the first window shown in Picking Terminal. Now showing the correct picked quantity.

* metasfresh-webui-frontend
  * [#2007](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2007) Dropdown fields too small in several places
    * Fixes the Dropdown width and length in Lookup and Dropdown widgets.
  * [#2018](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2018) Included view: clicking on it's right side space shall not close the included view
    * Navigation improvement in WebUI modal overlay. Now not closing the modal overlay anymore when the user clicks on white space of the included view.
  * [#2034](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2034) Uncaught TypeError: selected.indexOf is not a function
    * Internal bugfix in WebUI.
  * [#2036](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2036) Uncaught TypeError: Cannot read property 'length' of null at windowHandler (windowHandler.js:395)
    * Internal bugfix in WebUI.

# metasfresh 5.79
## Features

* metasfresh
  * [#4577](https://github.com/metasfresh/metasfresh/issues/4577) New Picking&Packing Workflow
    * Additional/ Alternative Picking and Packing Workflow.
  * [#4685](https://github.com/metasfresh/metasfresh/issues/4685) Order checkup with barcode report - add containers as separate fields
    * Improved Barcode Support for order checkup report in Manufacturing.
  * [#4687](https://github.com/metasfresh/metasfresh/issues/4687) Introduce and use PInstanceId object
    * Internal Improvement. New Process Instance Object.
  * [#4692](https://github.com/metasfresh/metasfresh/issues/4692) RabbitMQ: we shall use guest user by default
    * Improved RabbitMQ usage. Now using a guest user instead of metasfresh user.
  * [#4693](https://github.com/metasfresh/metasfresh/issues/4693) Validate ReadonlyLogic, MandatoryLogic and DisplayLogic
    * Application Dictionary improvement, now validating the entries in Readonly-, Mandatory and Display-Logic.
  * [#4700](https://github.com/metasfresh/metasfresh/issues/4700) Allow appending additional PDF-attachments to invoice-PDF
    * Extension of the Invoice PDF Document creation. Now it's possible to append an already created PDF to the Invoice PDF.

* metasfresh-webui-frontend
  * [#1933](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1933) Frontend shall ALWAYS use server's time zone
    * Switching the frontend behavior, now always using the Server's timezone.
  * [#2013](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2013) View: don't open row details if it's not allowed
    * Enhancement of frontend row open behavior. It's possible to define if a row shall be opened or not via doubleclick.
  * [#2020](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2020) View editing: fetch quickActions after PATCH /edit
    * Internal, general enhancement of the fetching of Quick Actions.

## Fixes
* metasfresh
  * [#4177](https://github.com/metasfresh/metasfresh/issues/4177) Performance bottleneck at Cache Invalidation
    * Improvement of Cache invalidation, removing a performance bottleneck.
  * [#4652](https://github.com/metasfresh/metasfresh/issues/4652) AD Element Translations leads to wrong fieldname Translations
    * Fixes the Translation update mechanism via Application Dictionary System Elements.
  * [#4683](https://github.com/metasfresh/metasfresh/issues/4683) Shipment Schedule does not set QtyToDeliver properly
    * Fix for Shipment Schedule. Now updateing the Quantity to deliver properly for product entries with isStocked = N masterdata configuration.
  * [#4696](https://github.com/metasfresh/metasfresh/issues/4696) Follow up #4552 AD_User is wrong in shipment schedule when using isDropShip
    * Further improvement of the Shipment Contact in Document Address generation in Sales Order Confirmation.
  * [#4704](https://github.com/metasfresh/metasfresh/issues/4704) Swing Picking Terminal: cannot write upper/lower case passwords when logging to Swing Picking Terminal
     * Bugfix for the Picking Terminal in Swing Client. Now it's possible to login with upper and lowercase password elements again.

* metasfresh-webui-api
  * [#1064](https://github.com/metasfresh/metasfresh-webui-api/issues/1064) Time switches when setting Preparation Date-Time
    * Improvement in WebUI Frontend for the Date and Timezone relevant data entries.
  * [#1074](https://github.com/metasfresh/metasfresh-webui-api/issues/1074) Process picking action not working
    * Bugfix in Picking workflow, now it's possible to Use the Process picking action again.
  * [#1075](https://github.com/metasfresh/metasfresh-webui-api/issues/1075) Unpick action not working
    * Bugfix in Picking workflow, now it's possible to Use the Unpick action again.
  * [#1076](https://github.com/metasfresh/metasfresh-webui-api/issues/1076) Cannot create a new sales order because "DeliveryViaRule is not set"
    * Fix for the Sales Order creation.

* metasfresh-webui-frontend
  * [#2021](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2021) Modal view: fetch quickActions on open; fetch quickActions when no selection
    * Improvement in WebuI Frontend when fetching Quickactions without selected rows.
  * [#2030](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2030) Errors when opening table views
    * Improving the Handling of missing data in WebUI Frontend.

# metasfresh 5.78
## Features

* metasfresh
  * [#4621](https://github.com/metasfresh/metasfresh/issues/4621) Support forum-datenaustausch.ch XML invoice
    * Implementation of the forum-datenaustausch.ch XML invoice for swiss helathcare document transactions.
  * [#4653](https://github.com/metasfresh/metasfresh/issues/4653) WebUI: Add missing Translations for en_US in Businesspartner Window
    * Switched Translations to ad_element for Business Partner Window.
  * [#4665](https://github.com/metasfresh/metasfresh/issues/4665) Show the Product No of Vendor in Purchase Order
    * Adjustment of the Purchase Order Document, now showing the Vendor Product No instead of the own Product No on Purchase Order Document.
  * [#4673](https://github.com/metasfresh/metasfresh/issues/4673) Enlarge AD_Process.SQLStatement to fit large SQL queries
    * Resizing the Process SQL Statement to allow large SQL Queries.
  * [#4677](https://github.com/metasfresh/metasfresh/issues/4677) Enable zoom to invoice candidates
    * Enables the Zoom to Reference for Invoice Candidates.
  * [#4547](https://github.com/metasfresh/metasfresh/issues/4547) Sales order based process for contract extension
    * New Process that allows to extend contracts and update the contract status tp show active, prolonged and cancelled contracts.

* metasfresh-webui-api
  * [#1033](https://github.com/metasfresh/metasfresh-webui-api/issues/1033) API for "About" action in webui
    * New API for the Created and Updated Infos for a selected record.
  * [#1055](https://github.com/metasfresh/metasfresh-webui-api/issues/1055) Include internalName in JSONDocumentAction
    * Includes the Internal Name (window and tabs) to WebUI Frontend. These names can be used for automated frontend tests.
  * [#1072](https://github.com/metasfresh/metasfresh-webui-api/issues/1072) Implement REST endpoints for managing migration scripts
    * New Functionality, that allows the creation of migration scripts via WebUI Frontend.
  * [#1069](https://github.com/metasfresh/metasfresh-webui-api/issues/1069) View: have a way to define if views support opening row details
    * Internal improvement of the opening of rows in WebUI frontend. Now the backend tells how to behave in such cases.

* metasfresh-webui-frontend
  * [#1989](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1989) Hourglass Overlay for pending Posts
    * Now showing a Loading indicator for windows with a large amount of records, to indicate about waiting time.
  * [#2005](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2005) Allow decimal comma in Qty Fields
    * New Number component that allows to record numbers with decimal point or comma.
  * [#2009](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2009) Views: Automatically remove view rows if GET /byIds it's not returning the row(s) frontend asked for
    * Improvement in Frontend, removing rows automatically when API does not return them.
  * [#2014](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2014) Views: refresh `quickActions` after `GET /byIds`
    * Improvement in Frontend, now refreshing quickactions after row changes.

## Fixes

* metasfresh
  * [#4671](https://github.com/metasfresh/metasfresh/issues/4671) WebUI Picking does not return filtered HU for selection
    * Bugfix in Picking Terminal, when not returning the filtered Handling Unit although selected via Parameter.

* metasfresh-webui-api
  * [#1067](https://github.com/metasfresh/metasfresh-webui-api/issues/1067) Attributes Filter in Picking shall work on load as before
    * Bugfix in Picking Terminal for Quick Actions not shown on load.
  * [#1068](https://github.com/metasfresh/metasfresh-webui-api/issues/1068) Cannot add orderline using "Add new", error when selecting product
    * Fixes an issue in Orderline creation using "Add new" line action.

* metasfresh-webui-frontend
  * [#2016](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2016) Indicator bar not visible
    * Bugfix and Improvement for the Save Status Indicator.

# metasfresh 5.77
## Features

* metasfresh
  * [#4567](https://github.com/metasfresh/metasfresh/issues/4567) Automatic Lot No. Handling into Quarantine Warehouse
    * New Quarantine Handling Feature in Material Receipt.
  * [#4609](https://github.com/metasfresh/metasfresh/issues/4609) HUEditor-Tweaks
    * Adjustments to the Handlign Unit Editor window.
  * [#4628](https://github.com/metasfresh/metasfresh/issues/4628) Split material dispo for M_Transaction with different attributes
    * Improvement of the ATP Calculation for Transactions that were not fulfilled same as planned.
  * [#4633](https://github.com/metasfresh/metasfresh/issues/4633) Generic Process for SQL -> Excel Export
    * New Feature that allows to create SQL Actions and add them to WebUI Menu or Windows for Excel Export.
  * [#4636](https://github.com/metasfresh/metasfresh/issues/4636) Support attachments being linked to multiple records
    * New Functionality that allows to add attachments references to multiple records.
  * [#4640](https://github.com/metasfresh/metasfresh/issues/4640) Option to remove M_Product_Category_ID from Material Cockpit
    * New Option for Material Cockpit that allows to remove the Product Category in grid and main View.
  * [#4646](https://github.com/metasfresh/metasfresh/issues/4646) Rename and extend AD_MigrationScript helper function
    * Internal Improvement for the Migration Script creation and handling.
  * [#4646](https://github.com/metasfresh/metasfresh/issues/4649) BPartners FTS shall not be active by default
    * Switching off the new Business Partner Full Text Search by default.
  * [#4659](https://github.com/metasfresh/metasfresh/issues/4659) Configurable Mailtext for Documents in DocOutbound
    * New Feature that allows to configure Mailtexts for Outbound Documents.

* metasfresh-webui-api
  * [#1063](https://github.com/metasfresh/metasfresh-webui-api/issues/1063) Global QR Code Actions support
    * New Barcode Feature that allows to Scan a QR Barcode in WebUI via Webcam now.
  * [#1066](https://github.com/metasfresh/metasfresh-webui-api/issues/1066) Don't show KPIs if the ElasticSearch system is disabled
    * New Configuration feature that allows to hide the KPI's on main Dashboard if Elastic Search service is not enabled.


* metasfresh-webui-frontend
  * [#1952](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1952) Advanced tooltip support
    * New Feature that allows to show advanced tooltips in WebUI frontend.
  * [#1955](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1955) Get rid of GET plugins.js 404 Not Found console error
    * Eliminating the error in console log for missing plugins.js.
  * [#1958](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1958) Use user language for messages and errors in Forgot Password feature (frontend)
    * Improvement of User Messages translation in Forgot Password workflow.
  * [#1972](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1972) Support active indication for filters without parameters
    * Extended functionality for the new Filter Features. Here improving Filter behavior for Filters with undisplayed filter parms.
  * [#1975](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1975) GitHub report about security vulnerability in twbs / bootstrap
    * Updating bootstrap to new version because of security issue.
  * [#1978](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1978) Make actions cypress friendly
    * Improvement of Cypress Testing in metasfresh WebUI.
  * [#1981](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1981) Make composite widget fields cypress friendly
    * Improvement of Cypress Testing in metasfresh WebUI.
  * [#1983](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1983) Height of date fields is off
    * Fixing the height of Date Fields.
  * [#1985](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1985) Make tooltip icons always visible
    * Showing the Lookup Fields Tooltips now also when the Field is readonly.
  * [#1987](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1987) Adjustments to tooltip widget
    * Layout Improvements for the new Tooltip widget.
  * [#1990](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1990) QR code support
    * New Feature that allows to scan QR Codes now.
  * [#1999](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1999) Process execution result action: render QR code
    * New Feature in WebUI that allows to scan QR Barcodes.

## Fixes

* metasfresh
  * [#4625](https://github.com/metasfresh/metasfresh/issues/4625) Open Items List Reference Date wrong parm
    * Fix for the Open Items Reference Date Parm, now able to select to Open Items to a specific date again.
  * [#4632](https://github.com/metasfresh/metasfresh/issues/4632) Swing Picking Terminal: cannot pick
    * Bugfix for a minor case in Picking Workflow.
  * [#4644](https://github.com/metasfresh/metasfresh/issues/4644) Clone Quotation, switch Sales Order. Wrong Document No
    * Improvement of the Sales Order Clone Feature. Now switching the Document No Sequence if Doctype is changed.
  * [#4650](https://github.com/metasfresh/metasfresh/issues/4650) Elasticsearch shall use slf4j instead of log4j (again)
    * Improvement of the Elasticsearch logging. Switched to another logger.
  * [#4657](https://github.com/metasfresh/metasfresh/issues/4657) AD_Message cache in Msg not invalidated on data change
    * Cache Invalidation Improvement for WebUI.
  * [#4658](https://github.com/metasfresh/metasfresh/issues/4658) Dunning jasper uses untranslated _trl records
    * Fixed the Translation prossibility of Jasper Dunning Documents.

* metasfresh-webui-api
  * [#1060](https://github.com/metasfresh/metasfresh-webui-api/issues/1060) Allow parent-link relation to be set in AD_Tab
    * Application Dictionary improvement, now allowing parent link relations to be set in Tab Configuration.

* metasfresh-webui-frontend
  * [#1975](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1975) GitHub report about security vulnerability in twbs / bootstrap
    * Fixes a Vulnerability Report about bootstrap.
  * [#1992](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1992) Ugly double border when editing in Date Fields
    * Adjustment of the Border Layout for mandatory Date Fields.
  * [#1993](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1993) Date Icon moved few pixels to left for mandatory
    * Alignment improvement for Calendar Icons in mandatory Date Fields.
  * [#1995](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1995) Cypress Test: Manufacturing Order Test fails
    * Bugfix for failing Manufacturing Order Test with Cypress.
  * [#1998](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1998) Open view process action shall support profileId (frontend)
    * Fix in WebUI Frontend when opening a View. Now the ProfileID is used when opening a View.
  * [#2000](https://github.com/metasfresh/metasfresh-webui-frontend/issues/2000) Modal view shall query the quick actions initially
    * Bugfix when opening Modal Views initially. Now the Quick Actions are queried too.

# metasfresh 5.76
## Features
* metasfresh
  * [#4582](https://github.com/metasfresh/metasfresh/issues/4582) Excel Export and SQL for Product Specifications
    * New Excel Export for a Product Specifications sheet.
  * [#4601](https://github.com/metasfresh/metasfresh/issues/4601) Allow activating spring profiles via AD_SysConfig
    * New Feature that allows to activate Spring Profiles via System Configuration.
  * [#4605](https://github.com/metasfresh/metasfresh/issues/4605) Webui: Org window: hide the AD_Org_ID field
    * Hiding the Organisation Field in Organisation Window.
  * [#4610](https://github.com/metasfresh/metasfresh/issues/4610) Billto Location and contact override in invoicecandidates
    * New Possibility to overwrite Billto Location and Contact via Invoice Candidates.
  * [#4619](https://github.com/metasfresh/metasfresh/issues/4619) de.metas.util - Rename packages to de.metas.util
    * Internal housekeeping improvement.

* metasfresh-webui-api
  * [#1049](https://github.com/metasfresh/metasfresh-webui-api/issues/1049) Pipes/Cabling quick input shall not display the BOM products
    * Improvement of the cable batch entry mode, now not showing the Bill of Materials anymore.

* metasfresh-webui-frontend
  * [#1926](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1926) Make window tabs cypress friendly
    * Improvement of WebUI Tab Names, making it easie to use them in Cypress Test instructions.
  * [#1957](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1957) On password reset, show the error message
    * Enhancing the error messages in Forgot Password workflow.

## Fixes

* metasfresh
  * [#4599](https://github.com/metasfresh/metasfresh/issues/4599) Error when posting a zero-sum invoice
    * Bugfix for the posting of zero-sum invoices.
  * [#4622](https://github.com/metasfresh/metasfresh/issues/4622) Requests can not be saved II
    * Bugfix for the saving of Requests in Subtabs.
  * [#4624](https://github.com/metasfresh/metasfresh/issues/4624) Invoice candidate not updated after shipment reactivate and complete
    * Fixes the invoice candidate invalidation when reactivating and completing a shipment.

* metasfresh-webui-api
  * [#1051](https://github.com/metasfresh/metasfresh-webui-api/issues/1051) New Org cannot be created anymore
    * Fixes the Org creation in WebUI.

* metasfresh-webui-frontend
  * [#1949](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1949) Shortcuts not working properly in Tabs after changing sth in grid view + [Tab]
    * Improvement of Shortcut Handling after Delete in Subtab.
  * [#1972](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1972) Support active indication for filters without parameters
    * Improvement of Filters in WebUI, now indicating also active Filters without parameters.

# metasfresh 5.75
## Features
* metasfresh
  * [#4507](https://github.com/metasfresh/metasfresh/issues/4507) Picked and Non-Picked Quantities Shipment generation
    * New action available in Shipment Schedules. Now it's possible to create shipments that include picked quantities and non-picked quantities as fallback scenario.
  * [#4549](https://github.com/metasfresh/metasfresh/issues/4549) Sales Order Candidates REST API improvements
    * Improvements of the REST API endpoint for Sales Order Candidates.
  * [#4556](https://github.com/metasfresh/metasfresh/issues/4556) Show Product note as tooltip in order line
    * Adding a Toltip functionality for Products in Orderline.
  * [#4557](https://github.com/metasfresh/metasfresh/issues/4557) Improve BPartner Memo-Import
    * Improves the Data Import of Business Partner Memo fields.
  * [#4558](https://github.com/metasfresh/metasfresh/issues/4558) Show BPartner memo as tooltip in order
    * Adding a Toltip functionality for Business Partner in Order Header.
  * [#4566](https://github.com/metasfresh/metasfresh/issues/4566) Save AdempiereProcessor lastRun/nextRun timestamp out-of-trx
    * Internal Housekeeping improvement for ADempiere Processor.
  * [#4568](https://github.com/metasfresh/metasfresh/issues/4568) Add note field to invoice candidates
    * Adding a Tooltip functionality in Invoice Candidates.
  * [#4575](https://github.com/metasfresh/metasfresh/issues/4575) Allow custom, POReference-based document number
    * New Feature that allows a custom document/ sequence number based on Purchase Order Reference.
  * [#4576](https://github.com/metasfresh/metasfresh/issues/4576) Introduce Warehouse Type
    * Improvement of Warehouse configuration. Now it's possible to define warehouse types and add types to warehouses.
  * [#4587](https://github.com/metasfresh/metasfresh/issues/4587) Allow custom PDF-creating code to be called via print-format
    * New Extension that allows to use custom code for PDF Creation via Print Format.
  * [#4593](https://github.com/metasfresh/metasfresh/issues/4593) MailWorkpackageProcessor shall mail the AD_Archive's own PDF
    * Adjustment of the Mail Workpackage Processor, now mailing the Archives PDF instead regenerating the PDF from Document.
  * [#4594](https://github.com/metasfresh/metasfresh/issues/4594) WebUI: Outbound EMail Server (SMTP)
    * New Window for the Outbound eMail Server Configuration in WebUI.
  * [#4595](https://github.com/metasfresh/metasfresh/issues/4595) WebUI: Window EMail Server Routing
    * New Window for the eMail Server Routing Configration in WebUI.
  * [#4613](https://github.com/metasfresh/metasfresh/issues/4613) Provide doc-outbound mail receiver for dunning docs
    * Extension of Document Outbound, now also setting a Mail Receiver User for Dunning Documents.
  * [#4615](https://github.com/metasfresh/metasfresh/issues/4615) Turn C_DunningDoc into a real document
    * Transforming the Dunning Documents into real document model of metasfresh.

* metasfresh-webui-api
  * [#1038](https://github.com/metasfresh/metasfresh-webui-api/issues/1038) Use user language for messages and errors in Forgot Password feature
    * Translation of User Messages during the "Forgot Password Feature" workflow.

## Fixes

* metasfresh
  * [#4563](https://github.com/metasfresh/metasfresh/issues/4563) Sometimes missing purchase candidates aren't created
    * Fixes a cornercase of missing Purchase Candidates.
  * [#4579](https://github.com/metasfresh/metasfresh/issues/4579) MSV3 - local purchase order is not created if remote order confirmation lacks deliveryDate
    * Fix for the Pharma MSV3 Purchase order creation.
  * [#4591](https://github.com/metasfresh/metasfresh/issues/4591) Printing problem on multi-org-system
    * Configuration Fix for Printing on Multi Org Systems.
  * [#4592](https://github.com/metasfresh/metasfresh/issues/4592) Number Format Exception
    * Fixes a Number Fomat Exception in Webcam Foto Upload of Material Receipt Candidates.
  * [#4602](https://github.com/metasfresh/metasfresh/issues/4602) Cannot complete flatrate term conditions / transition in swing
    * Fixes a Null Pointer Exception in metasfresh Swing Client when completing flatrate term conditions.
  * [#4623](https://github.com/metasfresh/metasfresh/issues/4623) Invoice candidate recompute flag not always removed in webui
    * Fixes the behavior of the Invoice Candidate recompute flag for some minor cases.
  

* metasfresh-webui-api
  * [#1046](https://github.com/metasfresh/metasfresh-webui-api/issues/1046) Sometimes there are no available DocActions for Sales Orders
    * Adjusting the retrieval of possible Document Actions, avoiding cornercases that these were sometimes not shown in WebUI Documents.
  * [#1047](https://github.com/metasfresh/metasfresh-webui-api/issues/1047) Allow purchase disposition from sales order only for drafted sales orders
    * Restricting the usage of purchase disposition from Sales Orders, now only for drafted sales Orders.

* metasfresh-webui-frontend
  * [#1944](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1944) Filter for attributes in picking terminal is not set on Y altough should be
    * Fix for the Handling Unit Panel default filtering in Picking Terminal.
  
# metasfresh 5.74
## Features

* metasfresh
  * [#4411](https://github.com/metasfresh/metasfresh/issues/4411) New Dunning trigger for flatrate terms
    * Extended Dunning Feature, now calculating the invoice due date from flatrate terms due date.
  * [#4516](https://github.com/metasfresh/metasfresh/issues/4516) New Action "Copy Window"
    * Enhance Application Dictionary Feature allowing to copy window configurations for webui.
  * [#4524](https://github.com/metasfresh/metasfresh/issues/4524) Implement inbound E-Mail support
    * New Feature that supports inbound eMail communication now.
  * [#4541](https://github.com/metasfresh/metasfresh/issues/4541) Return also URL using function de_metas_endcustomer_fresh_reports.Docs_Generics_Org_Report
    * Enhancing the function Docs_Generics_Org_Report, now returning the URL too.
  * [#4550](https://github.com/metasfresh/metasfresh/issues/4550) Show Pricing Condition Indicator in Purchase Orders
    * Including the Pricing Condition Indicator, known from Sales Orderline, in Purchase Orderline too.
  * [#4554](https://github.com/metasfresh/metasfresh/issues/4554) Process to create dunning-PDF with concatenated invoice-PDFs
    * New Process that allows to concatenate Dunning Documents with invoice PDF's.
  * [#4561](https://github.com/metasfresh/metasfresh/issues/4561) QueryStatisticsLogger shall use logger instead of stderr
    * Now Logging out SQL infos instead of printing them to stderr. 

* metasfresh-webui-api
  * [#1035](https://github.com/metasfresh/metasfresh-webui-api/issues/1035) Implement CORS support
    * New feature, now supporting cross origin resource sharing.
  * [#1037](https://github.com/metasfresh/metasfresh-webui-api/issues/1037) Advanced tooltip support
    * New Functionality now supporting advanced tooltips in webui.

* metasfresh-webui-frontend
  * [#1908](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1908) Show multiple lines of a multi line text field in grid tab
    * New feature that expands multiline fields when the row is selected.
  * [#1953](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1953) Show field-description in tool-tip instead of field-caption
    * New Feature that shows the Field Description instead of Caption when hovering in webui.

## Fixes

* metasfresh
  * [#4528](https://github.com/metasfresh/metasfresh/issues/4528) Can not add new scale price on 5.71
    * Fixes a Bug in Product Prices when recording Scale Prices.
  * [#4552](https://github.com/metasfresh/metasfresh/issues/4552) AD_User is wrong in shipment schedule when using isDropShip
    * Fixes the Shipment Contact User when using Drop Shipment in Sales Order.
  * [#4560](https://github.com/metasfresh/metasfresh/issues/4560) MSV3 related fixes
    * Fixes different Pharma MSV3 related issues.
  * [#4572](https://github.com/metasfresh/metasfresh/issues/4572) Texts missing in cloned sales quotation
    * Bugfix for Document Line descriptions when closing Sales Orders/ Quotations.

* metasfresh-webui-api
  * [#1040](https://github.com/metasfresh/metasfresh-webui-api/issues/1040) Some views are failing because #AD_User_ID was not found in context
    * Bugfix in WebUI. Views with #AD_User_ID context are now not failing anymore.
  * [#1043](https://github.com/metasfresh/metasfresh-webui-api/issues/1043) Open PDF from Printing Queue stopped working
    * Fixes a Bug when opening a PDF from Printing Queue. Nw the PDF is opened again.

* metasfresh-webui-frontend
  * [#1898](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1898) No results when clicking on the looking glass button
    * Fixes the cursor hovering magnifying glass icon. Now shown as default cursor.
  * [#1931](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1931) Hint for shortcut [alt]+u not displayed anymore when hovering over the resp. button
    * Now shows the Quickaction Tooltip again.
  * [#1932](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1932) Mandatory Field not filled Error too early
    * Fixes the UI Error Handling for mandatory Fields.
  * [#1935](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1935) Tab shall be usable to navigate through the dropdown sequence in combined Business Partner Lookups
    * Bugfix for the Tab Handling in combined Lookup Fields. Now it's possible to navigate with [tab] again.
  * [#1944](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1944) Filter for attributes in picking terminal is not set on Y altough should be
    * Fixes the initial settings of filter parameters in webui.

# metasfresh 5.73
## Features

* metasfresh
  * [#4475](https://github.com/metasfresh/metasfresh/issues/4475) Refund contract - add further options
    * Extended Functionality added to Refund contracts enabling enhanced calculations.
  * [#4511](https://github.com/metasfresh/metasfresh/issues/4511) Implement support for MSV3 version 1
    * Extended MSV3 Functionality. Now allowing the usage of MSV3 version 1 too.
  * [#4521](https://github.com/metasfresh/metasfresh/issues/4521) Don't create subscription shipment schedules for products that are no items
    * Enhanced subscription handling. Not creating shipment schedules anymore for non item Products.
  * [#4530](https://github.com/metasfresh/metasfresh/issues/4530) WebUI Adjustments for Country, Postal and City Window
    * New Window in WebUI, allowing to maintain Country, Postals and Cities.
  * [#4535](https://github.com/metasfresh/metasfresh/issues/4535) Set Sales Order Line's ProductDescription as Product BOM's description
    * Enhanced Feature for Cable Trade Verticals. Now adding the BOM Components in Prodtct Description Field in Sales Orderline.
  * [#4536](https://github.com/metasfresh/metasfresh/issues/4536) Introduce AD_Table.IsEnableRemoteCacheInvalidation
    * New Configuration Feature in Application dictionary. It is now possible to enable/ disable the Remote Cache Invalidation for a Table.

metasfresh-webui-api
  * [#1032](https://github.com/metasfresh/metasfresh-webui-api/issues/1032) Window layout API shall provide text multilineText and multilineTextLines properties
    * New Multiline Fature in WebUI Frontend. When selecting grid lines with multiline Fields, than the lineheight is automatically expanded.

## Fixes
* metasfresh
  * [#4520](https://github.com/metasfresh/metasfresh/issues/4520) Requests cannot be saved
    * Fixes a Bug in Requests, now being able to save Requests again in WebUI.
  * [#4523](https://github.com/metasfresh/metasfresh/issues/4523) Fix problems with invoice candidate creation from subscription flatrate terms
    * Bugfix in subscription contract handling, now creating corresponding invoice candidates again.
  * [#4526](https://github.com/metasfresh/metasfresh/issues/4526) Filter for attributes in picking terminal shall be set by default
    * Bugfix for the extended User Filter Features. Now possible to set default user filter parms again.
  * [#4537](https://github.com/metasfresh/metasfresh/issues/4537) Invoice candiate handler BL creates lock with non-unique owner
    * Internal Bugfix for the Invoice Candidate handler Business Logic.
  * [#4538](https://github.com/metasfresh/metasfresh/issues/4538) WebUI: New Translation Window for R_RequestType
    * New Window that allows to maintain Request Type Translations in WebUI.

* metasfresh-webui-api
  * [#438](https://github.com/metasfresh/metasfresh-webui-api/issues/438) Minor: error for wizard with no picture
    * Fixes a Bug in Organisation Setup Wizard when no Logo Image is present.

# metasfresh 5.72
## Features
* metasfresh
  * [#4448](https://github.com/metasfresh/metasfresh/issues/4448) Advanced BLs to create inventory lines
    * Extended Business Logic for the creation of Inventory lines. Now able to generate the inventorylines based on product value and last inventory count of products in a warehouse locator.
  * [#4450](https://github.com/metasfresh/metasfresh/issues/4450) Tablet optimized inventory-counting-window
    * New window that allows the invntory counting via a tablet sized interface.
  * [#4482](https://github.com/metasfresh/metasfresh/issues/4482) Support Doctype Text templates also on purchase order
    * Adopting the existing doctype text support to purchase orders.
  * [#4492](https://github.com/metasfresh/metasfresh/issues/4492) Project Status and Product Category Trl
    * New Translation Feature for Project Status and Product Category.
  * [#4494](https://github.com/metasfresh/metasfresh/issues/4494) Projecttype Org Validation
    * New Validation Rule for Projecttype, now respecting the records organisation.
  * [#4498](https://github.com/metasfresh/metasfresh/issues/4498) Make fields in explicit user filter mandatory or optional
    * Extended Filter functionality allowing to set
  * [#4501](https://github.com/metasfresh/metasfresh/issues/4501) LogicExpressionEvaluator: improve error message in case something went wrong
    * Improvement of Error messages.
  * [#4517](https://github.com/metasfresh/metasfresh/issues/4517) Extend Sales Order REST API to support price and support all product values
    * Extended Sales Order REST API, now supporting prices and product values.

* metasfresh-webui-frontend
  * [#1878](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1878) Forgot password feature
    * New Feature that allows a User to reset a forgotten password.

## Fixes
* metasfresh
  * [#4483](https://github.com/metasfresh/metasfresh/issues/4483) Payment allocation form does not show invoices
    * Fix for the Payment Allocation Form, now showing filtered invoices again.
  * [#4499](https://github.com/metasfresh/metasfresh/issues/4499) Cannot create letter
    * Bugfix. Fixes the creation of Letters in WebUI modal overlay.
  * [#4504](https://github.com/metasfresh/metasfresh/issues/4504) Mandatory logic broken for C_FlatrateTerm.C_Currency_ID
    * Fixes the evaluation of the mandatory logic for the Currency Field in Flatrate Term window.
  * [#4506](https://github.com/metasfresh/metasfresh/issues/4506) Compensation Group's subtotals gets broken after setting/changing the flatrate conditions
    * Bugfix for the calculation of the subtotal in compensation groups. Now these are recalculated when adjusting corresponding flatrate conditions.
  * [#4509](https://github.com/metasfresh/metasfresh/issues/4509) NPE in Compensation Groups creation
    * Bugfix for a Null Pointer Exception when creating compensation groups in Sales Order Lines.
  * [#4514](https://github.com/metasfresh/metasfresh/issues/4514) Include sales orders REST API to metasfresh-dist/serverRoot
    * Invluding the REST API for Sales Orders to default API environment.

* metasfresh-webui-frontend
  * [#1188](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1188) Home and End button move caret in text fields
    * Bugfix for the Keyboard support of [home] and [end] keys in Text Fields.
  * [#1463](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1463) Unable to execute any quick actions in Firefox
    * Fixes a Bug that occurred with quickactions in non-webkit browsers.
  * [#1578](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1578) Applied filter params sometimes not displayed in filter
    * Minor Bugfix for the filtering in WebUI window.
  * [#1589](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1589) Included tab: when refreshing via websocket event the sort/order is not preserved
    * Improvement of the Websocket refresh behavior when manipulating records in combination with changed order.
  * [#1707](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1707) Red line is missing when a document was not saved
    * Improvement of the Error Handling for Records that cannot be saved.
  * [#1872](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1872) [alt]+u not working as before
    * Fix for the Shortcut [alt]+u.
  * [#1923](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1923) Sequence of Dropdowns in combined Business Partner Lookups not working
    * Bugfix for the automatic workflow sequence of combined Lookup Fields.
  * [#1927](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1927) No additional filter parameter from a dropdown selectable when filter has a default value set
    * Fixes the Filtering in WebUI for filters that have a default filter criteria set. Now it's possible to also set other filter criteria again.
  * [#1934](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1934) Cannot run processes
    * Bugfix for running actions with parameters.
  * [#1948](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1948) Filter Attribute Label not set properly
    * Fixes the Filter Button Label.
    

# metasfresh 5.71
## Features
* metasfresh
  * [#4459](https://github.com/metasfresh/metasfresh/issues/4459) Material Cockpit - show stock details
    * New Feature in Material Cockpit, now showing the Stock details and Locators.
  * [#4491](https://github.com/metasfresh/metasfresh/issues/4491) Introduce Window Tab's Internal Name
    * New internal Functionality in Application Dictionary that allows to define internal Names of window Tabs for automatic Testing purpose.

## Fix
* metasfresh-webui-api
  * [#865](https://github.com/metasfresh/metasfresh-webui-api/issues/865) Org * not selectable in WebUI but in Java Client
    * Fix of API now allowing to record Org * in Records.
  * [#1027](https://github.com/metasfresh/metasfresh-webui-api/issues/1027) Cannot set attributes for product after receipt in manufacturing
    * Bugfix for the setting of Attributes after doing a Material Receipt.

* metasfresh-webui-frontend
  * [#1672](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1672) Location dropdown opens again when opening the batch entry
    * Fixes the Lookup behavior in Sales Order Batch entry.


# metasfresh 5.70
## Features
* metasfresh
  * [#4444](https://github.com/metasfresh/metasfresh/issues/4444) Refund Flatrate Terms adjustments
    * New Notification Feature for Refund Contracts, allowing to notify Users about ending contracts.
  * [#4467](https://github.com/metasfresh/metasfresh/issues/4467) Get rid of the legacy IProcess interface
    * Internal Housekeeping, removing Removes legacy code IProcess.

## Fix
* metasfresh
  * [#4463](https://github.com/metasfresh/metasfresh/issues/4463) Wrong pricelist when different invoice partner in sales order
    * Bugfix for Pricelist retrieval in Sales Order, now getting the correct Pricelist in cases of different Invoice Partners. 
  * [#4464](https://github.com/metasfresh/metasfresh/issues/4464) Report Business Partner revenue is not working anymore in swing
    * Fixes the Revenue Business Partner Report in swing client.

* metasfresh-webui-frontend
  * [#1911](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1911) Filters in HU Editor
    * Fix for the Web UI, now not cuting off Filter criteria anymore in narrow window situations.
  * [#1916](https://github.com/metasfresh/metasfresh-webui-frontend/pull/1916) Fix barcode scanner in HU editor
    * Fix for the Barcode Scanner in Handling Unit editor.
  * [#1672](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1672) Location dropdown opens again when opening the batch entry
    * Fixes a focus issue in Lookup fields.

# metasfresh 5.69
## Features
* metasfresh
  * [#4303](https://github.com/metasfresh/metasfresh/issues/4303) Extend webui for PaymentDiscount
    * New Feature that allows to set an override Payment Discout Rate via Sales Orderline.
  * [#4392](https://github.com/metasfresh/metasfresh/issues/4392) ESR RefNo too short after scan in Purchase Invoice action
    * Extended Feature for Reding the ESR Record No. in Invoice for No. that don't have default digits, now filling with leading zeroes.
  * [#4400](https://github.com/metasfresh/metasfresh/issues/4400) Fix zoom PrintingQueue=>PrintJob and others
    * New Zoom from Printing Queue to Print Jobs.
  * [#4419](https://github.com/metasfresh/metasfresh/issues/4419) Material Receipt Dispo Adjustment
    * Adjustments to Material Receipt Dispo Window and Functionality.
  * [#4423](https://github.com/metasfresh/metasfresh/issues/4423) Add vattaxid in Docs_Purchase_Order_Details_Sum function
    * Extended SQL Function, now adding the VAT Tax Id.
  * [#4437](https://github.com/metasfresh/metasfresh/issues/4437) Purchase order: Show description and description bottom
    * New Fields in Purchase Order for description and description bottom.
  * [#4454](https://github.com/metasfresh/metasfresh/issues/4454) Material Cockpit - add columns and allow to hide columns via config
    * Extended configuration possibility for Material Cockpit allowing to display/ hide columns.
  * [#4456](https://github.com/metasfresh/metasfresh/issues/4456) Material Cockpit - allow to configure the attribute detail rows' dimenstion spec
    * Extended Material Cockpit now having additional Fields.

* metasfresh-webui-frontend
  * [#1899](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1899) Improve quick/batch entry layout
    * New internal Feature that allows to set the sizes of Batch Entry Fields.
  * [#1909](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1909) Vertical Cabling : Show full product name on quick order entry
    * Enhanced Lookup Dropdown in Batch entry fields, now allowing to have the dropdown wider than the corresponding search Field.
  
## Fixes
* metasfresh
  * [#4426](https://github.com/metasfresh/metasfresh/issues/4426) Error on new purchase order
    * Bugfix for new Purchase Order creation with EDI Receipient involved.
  * [#4428](https://github.com/metasfresh/metasfresh/issues/4428) Missing lines in jasper documents
    * Bugfix for Jasper Documentline when Product Categories ane inactive.
  * [#4451](https://github.com/metasfresh/metasfresh/issues/4451) HU Editor in picking terminal shows all HUs: not filtered for product
    * Fixes a filtering Bug in Handling Unit editor, now only showing the entries for the filtered Product again.
  * [#4418](https://github.com/metasfresh/metasfresh/issues/4418) Report Revenue Business Partner without Attributes
    * Fix for Attributes in Shipment Schedule lines and for the Revenue Business Partner Report.

* metasfresh-webui-frontend
  * [#1887](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1887) Non mandatory blue fields in grid view
    * UI Improvement, now not showing a blue border for non-mandatory fields after initial edit.
  * [#1890](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1890) Applying filter params with [alt]+Enter not working in modal windows
    * Keyboard Shortcut adjustment, now allowing to use [alt]+enter in modal views with filter parameters.
  * [#1901](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1901) Highlighted action is not the one from mouse over when calling actions with [alt]+l
    * Shortcut fix for [alt]+l.

# metasfresh 5.68
## Features
* metasfresh
  * [#4092](https://github.com/metasfresh/metasfresh/issues/4092) sync mail address between contactperson and linked user
  * [#4153](https://github.com/metasfresh/metasfresh/issues/4216) Follow up : #4153 Serial Letter Feature
  * [#4323](https://github.com/metasfresh/metasfresh/issues/4323) Window Payment Allocations not editable
    * Making the Window for Payment Allocation now editable in webui.
  * [#4396](https://github.com/metasfresh/metasfresh/issues/4396) Pipes/Cabling vertical
  * [#4403](https://github.com/metasfresh/metasfresh/issues/4403) Process to void order and revert flatrate terms, shipment schedule, invoice candidates
  * [#4413](https://github.com/metasfresh/metasfresh/issues/4413) ShipmentScheduleHandler.retrieveModelsWithMissingCandidates() shall return an iterator
  * [#4416](https://github.com/metasfresh/metasfresh/issues/4416) Split Product Nutrition/ Allergene in 2 Tabs
  * [#4417](https://github.com/metasfresh/metasfresh/issues/4417) New Textfield for Product Ingredients without BOM

## Fixes
* metasfresh
  * [#1629](https://github.com/metasfresh/metasfresh/issues/1629) Invoice data goes missing in payment after save
  * [#4405](https://github.com/metasfresh/metasfresh/issues/4405) Action Sales Order from Quotation wrong Prices
  * [#4412](https://github.com/metasfresh/metasfresh/issues/4412) async-processors shall only run on app
  * [#4415](https://github.com/metasfresh/metasfresh/issues/4415) JSON Fehler "Der Kurier"

* metasfresh-webui-frontend
  * [#1889](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1889) Order line batch entry not working for current experimental cables/pipes batch entry
  * [#1895](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1895) closing address editor after entering only the country is not possible

# metasfresh 5.67 (2018-30)
## Features
* metasfresh
  * [#4292](https://github.com/metasfresh/metasfresh/issues/4292) Make a Webui-Window for HU Reservation
    * New Window for Handling Unit Reservation in WebUI.
  * [#4336](https://github.com/metasfresh/metasfresh/issues/4336) WebUI: add email fields to C_Doc_OutBound
    * New Fields and Filter criteria in Documentoutbound window in WebUI.
  * [#4376](https://github.com/metasfresh/metasfresh/issues/4376) Pricing engine sets the scale of price amounts to the respective precision
  * [#4380](https://github.com/metasfresh/metasfresh/issues/4380) consolidate profit related columns in order line and purchase candidate
  * [#4395](https://github.com/metasfresh/metasfresh/issues/4395) Notification if automatic TU label print failed

* metasfresh-webui-api
  * [#1010](https://github.com/metasfresh/metasfresh-webui-api/issues/1010) Implement process parameters callout support

* metasfresh-webui-frontend
  * [#1859](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1859) Inline rendering filter parameters
    * New Feature that allows inline rendering of Filter elements. This Feeature is used initially in the Fulltext Search Filter in Businesspartner Window.

## Fixes
* metasfresh
  * [#4172](https://github.com/metasfresh/metasfresh/issues/4172) Purchase order from sales order not working as before
  * [#4185](https://github.com/metasfresh/metasfresh/issues/4185) If C_DocType_Trl description exists, use this as description in document
  * [#4365](https://github.com/metasfresh/metasfresh/issues/4365) Error Zooming from material receipt to HU tracing
  * [#4371](https://github.com/metasfresh/metasfresh/issues/4371) Sales Order VAT vs. Invoice Candidate VAT

* metasfresh-webui-api
  * [#1007](https://github.com/metasfresh/metasfresh-webui-api/issues/1007) HU-Editor - Refresh after HU-changing process not working properly
  * [#1012](https://github.com/metasfresh/metasfresh-webui-api/issues/1012) Cannot use transform on a TU without LU in HU Editor

* metasfresh-webui-frontend
  * [#1785](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1785) Search field in Pricing conditions - keyboard selection
    * Improving the selection of Pricing Conditions via Keyboard.
  * [#1831](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1831) Fields in modal window are copied to the one in the back
    * Fixes a Bug in modals having modal field content getting copied to the underlying data structure.
  * [#1865](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1865) Patch not sent when you delete a text in grid view
    * Fixes the editing/ patching of content in text fields in grid view editing mode.
  * [#1867](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1867) Set qty to purchase to 0 when removed
    * Fixes the Purchase Dispo Functionality in Sales Order, now setting the Qty to 0 when removing the Puchased Qty.
  * [#1871](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1871) alt+Enter not working as before
    * Improvement of the shortcut [alt]+Enter in different modal views.
  * [#1876](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1876) Action confirmation without tab does not use the set Parms
    * Fixes the usage of keyboard in process parm windows. Now the parms are also taken when using alt+enter without previous tab usage.
  * [#1880](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1880) Cannot complete documents
    * Fixes the Docactions in Documents.
  * [#1891](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1891) sitemap no longer working on current master
    * Fixes an Issue in metasfresh Sitemap.


# metasfresh 5.66 (2018-29)
## Features
* metasfresh
  * [#1461](https://github.com/metasfresh/metasfresh/issues/1461) Improve User Password Hashing
    * Improvement of the Password Hashing Feature. Now Hashing with SHA512.
  * [#4009](https://github.com/metasfresh/metasfresh/issues/4009) Improve callout org.compiere.model.Callout_AD_Column
    * Improvement of Callout_AD_Column, making it WebUI friendly.
  * [#4026](https://github.com/metasfresh/metasfresh/issues/4026) Generate and mail the CSV only when Der Kurier shipper transportation is completed
    * Adjustment of the Shipper Transportation workflow for "Der Kurier". Now generating and mailing the csv aggregation only when the transportation order is completed.
  * [#4299](https://github.com/metasfresh/metasfresh/issues/4299) Jasper: Translations missing in en_US version
    * New en_US Translations added to Jasper Documents.
  * [#4315](https://github.com/metasfresh/metasfresh/issues/4315) metasfresh-app server fails to startup on a dev-machine
    * Internal improvement of the startup of the metasfresh-app server for development purposes.
  * [#4345](https://github.com/metasfresh/metasfresh/issues/4345) Make accounting async
    * Improvement of accounting, making it asynch. Needed for new Costing Engine.
  * [#4346](https://github.com/metasfresh/metasfresh/issues/4346) Individual sequences for products and projects
    * New Feature that allows to use Sequence No. for Projects and Products.
  * [#4354](https://github.com/metasfresh/metasfresh/issues/4354) Notify user on error creating document PDF
    * New Feature that informs the user via Notification when a PDF cannot be created.
  * [#4359](https://github.com/metasfresh/metasfresh/issues/4359) Set default values for new Integer and YesNo AD_Columns
    * Improvement in Applcation Dictionary, now setting default values for all Integer and Yes No Fields
  * [#4367](https://github.com/metasfresh/metasfresh/issues/4367) HU Transformation for LU, Packing Item and TU Qty default
    * Improvement of the HU Transformation Action, now setting default Parms for Transformation.

* metasfresh-webui-api
  * [#1006](https://github.com/metasfresh/metasfresh-webui-api/issues/1006) Forgot password webui api
    * New Feature via API that allows to trigger a workflow for forgotten user passwords.
  * [#1009](https://github.com/metasfresh/metasfresh-webui-api/issues/1009) Cleanup ADProcessDAO
    * New internal improvement on API side that is needed for the Transformation Action improvement.

## Fixes
* metasfresh
  * [#4356](https://github.com/metasfresh/metasfresh/issues/4356) Sales Orderline:ERROR: duplicate key value violates unique constraint "c_paymentterm_name"
    * Fixes a Bug when creating a new Line in Sales Order.
  * [#4370](https://github.com/metasfresh/metasfresh/issues/4370) M_ReceiptSchedule_Generate_M_InOuts error if M_ReceiptSchedule has Qty = 0
    * Fixes a Bug in the generation Process of Receipts in case the Receipt Schedule has a quantity of 0.

# metasfresh 5.65 (2018-28)
## Features
* metasfresh
  * [#4217](https://github.com/metasfresh/metasfresh/issues/4217) IFA Product Fields in Pharma Product readonly
    * Improvement of Pharma vertical in Product masterdata, now showing the fields readonly that are set by IFA Product Import.
  * [#4219](https://github.com/metasfresh/metasfresh/issues/4219) Import Datev Primanota for Payments, Allocations
    * New Import Feature for the German accounting Software DATEV. It's possible to import DATEV Primanota Payments now.
  * [#4220](https://github.com/metasfresh/metasfresh/issues/4220) Lot No. Control without mandatory Product ID
    * Improvement of the Lot No. Control Feature, now possible to record Lot No. without Mandatory Product ID. This allows to use the Feature also with Pharma Repack No.
  * [#4285](https://github.com/metasfresh/metasfresh/issues/4285) Invoice Document Outbound eMail enqueing
    * Improvement of the Mail enqueueing process via Document Outbound Window.
  * [#4308](https://github.com/metasfresh/metasfresh/issues/4308) Zoom from sales order to material dispo should open all referencing records
    * Improvement of the referenced Documents Link from Sales Order to material Disposition.
  * [#4311](https://github.com/metasfresh/metasfresh/issues/4311) Purchase schedules date: consider vendor lead time and non business days
    * New Feature for Purchase Candidate Calculation. Th Purchase Schedule Dates are now calculates based on vendor lead time and non business days.
  * [#4318](https://github.com/metasfresh/metasfresh/issues/4318) Split the current M_ShipmentSchedule_Update async queue processor
    * Performance Improvement for Shipment Schedules creation.
  * [#4320](https://github.com/metasfresh/metasfresh/issues/4320) Improve mass print oversight
    * Improved maintenance functionality for printing, making it much easier to support printing issue cases.
  * [#4340](https://github.com/metasfresh/metasfresh/issues/4340) REST API for creating sales orders and attaching files to them
    * New Endpoint for sales order creation and endpoint for file attachments so sales orders.

* metasfresh-webui-frontend
  * [#1857](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1857) Readonly next and previous page buttons
    * Pagination Improvement. Now deactivating previous/ next buttons in pagination on fist/ last page.

* metasfresh-dist
  * [#47](https://github.com/metasfresh/metasfresh-dist/issues/47) Provide standalone metasfresh-dist-report docker image
    * New Standalone docker image for distribution reports.
  * [#48](https://github.com/metasfresh/metasfresh-dist/issues/48) Provide standalone metasfresh-webui-frontend k8s dev deployment
    * New Standalone docker image for kubernetes webui frontend.

## Fixes
* metasfresh
  * [#4271](https://github.com/metasfresh/metasfresh/issues/4271) Reactivated and completed sales order is considered as new sales order in Material Dispo
    * Fixes the Material Dispo entry creation after reactivating and completing sales Orders.
  * [#4276](https://github.com/metasfresh/metasfresh/issues/4276) HU Editor in picking terminal shows all HUs: not filtered for product, and HUs with status: Shipped
    * Fixes the Filtering in the Handling Unit Editor of Picking Terminal. Now only showing Handling Units that fit to the selected Product.
  * [#4284](https://github.com/metasfresh/metasfresh/issues/4284) Document Outbound eMail action
    * Fixes the Document Outbound eMail Action.
  * [#4307](https://github.com/metasfresh/metasfresh/issues/4307) Reversed material receipt not considered correctly in Material Cockpit
    * Bugfix for the Material Receipt reversal Handling in Material Cockpit.
  * [#4314](https://github.com/metasfresh/metasfresh/issues/4314) metasfresh-app server startup stalls if no activeMQ broker is available
    * Fixes the startup of App Server in cases n activeMQ broker is not available.
  * [#4342](https://github.com/metasfresh/metasfresh/issues/4342) ATP in batch entry is wrong after attributes are added
    * Fixes the Available to Pomise Quantity after adding attribute values to a Handling Unit.
  * [#4349](https://github.com/metasfresh/metasfresh/issues/4349) Error when creating a bpartner on the fly and not setting a name
    * Bugfix for the Business Partner creation via Sales Order window.

* metasfresh-webui-frontend
  * [#1467](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1467) Advanced Edit shortcut not working correctly
    * Improvement of the Handling of shortcuts.
  * [#1850](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1850) Initial Setup Wizard window's layout is distorted
    * Fixes the Layout of the Initial Setup Wizard
  * [#1858](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1858) Moving to next page in modal removes filters
    * Fixes the Pagination behavior in modal overlays.


# metasfresh 5.64 (2018-27)
## Features
  * [#3210](https://github.com/metasfresh/metasfresh/issues/3210) Manufacturing Issue action take exact qty from stock
    * New Feature in WebUI manufacturing, allowing to issue the based on planned Quantities.
  * [#4212](https://github.com/metasfresh/metasfresh/issues/4212) ATP Stock indicator in Sales Orderline
    * New Field in Sales Orderline that shows the ATP Stock.
  * [#4218](https://github.com/metasfresh/metasfresh/issues/4218) Pharma: DeliveryType B disallow Sales Orderline
    * New Feature for Pharma that restricts the Orderline creation for RX Products if the Customer does not have the permission to buy.
  * [#4221](https://github.com/metasfresh/metasfresh/issues/4221) Recording of Payment Discount instead of Payment Term
    * Possibility to record Payment Discounts instead of Payment Terms in Pricing Conditions.
  * [#4222](https://github.com/metasfresh/metasfresh/issues/4222) Pricing Conditions for all Products of a Manufacturer
    * New Feature that allows the recording or Pricing Conditions on all Products of a Manufacturer.
  * [#4223](https://github.com/metasfresh/metasfresh/issues/4223) Ban Manufacturer Products for a Businesspartner
    * Possibility to Ban all Products of a Manufacturer for a given Business Partner.
  * [#4224](https://github.com/metasfresh/metasfresh/issues/4224) Pharma: Additional Document/ Certificate Fields
    * New Certificate Fields for the Pharma Business Partner Window in WebUI.
  * [#4248](https://github.com/metasfresh/metasfresh/issues/4248) Details about HU attributes during sales order creation
    * New Feature that allows to see reserve Handling Units during Sales Orderline creation. The Handling Units are reserved in the needed Quanitity and provided in Picking as initial selection.
  * [#4252](https://github.com/metasfresh/metasfresh/issues/4252) Show c_bpartner memo field of Org BP in document footer
    * Enlarging the Business Partner Description to allow more Company Information in Document Footers.
  * [#4270](https://github.com/metasfresh/metasfresh/issues/4270) Purchase Order Document with up to 4 digits
    * Improveing the Purchase Order Document, allowing to use up to 4 digits for purchase prices.
  * [#4273](https://github.com/metasfresh/metasfresh/issues/4273) Copy BOM Consumer Label Fields to PP Order BOMLine
    * Copying the BOM Consumer Label Fields to the Manufacturing Order Bill of Material Line during Order complete.
  * [#4286](https://github.com/metasfresh/metasfresh/issues/4286) Allow repost eventlog with forcing handler to be processed again
    * New Feature that allows to report an event via the Window event log.
  * [#4293](https://github.com/metasfresh/metasfresh/issues/4293) WebUI: New Window for MSV3 Customer Window
    * New Window for Pharma MSV3 Server and Customer Configuration
  * [#4295](https://github.com/metasfresh/metasfresh/issues/4295) Avoid polluting the console by changing log level from INFO to DEBUG
    * Internal Housekeeping improvement, changing Info Level logging to debug level, reducing the amount of logging information in the console, when not needed.
  
## Fixes 
  * [#4282](https://github.com/metasfresh/metasfresh/issues/4282) Order line is flagged as Temporary Pricing Conditions when the conditions are actually missing
    * Fixes the setting of pricing conditions in Orderlines and introducing a new Flag for temporary pricing conditions.
  * [#4296](https://github.com/metasfresh/metasfresh/issues/4296) Only metasfresh-app shall ever start an embedded JMS broker
    * Internal improvement of starting embedded JMS broker, now only done by metasfresh-app.
  * [#4297](https://github.com/metasfresh/metasfresh/issues/4297) Exit when swing application context failed to initialize
    * Internal optimization, now exiting when the swing applicatiton fails to initialize the context.


# metasfresh 5.63 (2018-26)
## Features
* metasfresh
  * [#3772](https://github.com/metasfresh/metasfresh/issues/3772) EventBus shall use RabbitMQ instead of ActiveMQ
    * Switches the EventBus to use RabbitMQ instead of ActiveMQ from now on
  * [#4140](https://github.com/metasfresh/metasfresh/issues/4140) WebUI: Translation Window for Country
    * New Window for Country Translation maintenance.
  * [#4225](https://github.com/metasfresh/metasfresh/issues/4225) Pharma: Move Businesspartner Fields to Customer/ Vendor Tab
    * Improvement of the Pharma Business Partnmer Window in WebUI, rearranging customer and vendor Fields in their subtabs.
  * [#4237](https://github.com/metasfresh/metasfresh/issues/4237) Add UC constraints to C_Aggregation
    * Improvement of the Aggregation Performance.
  * [#4238](https://github.com/metasfresh/metasfresh/issues/4238) Implement full text search for BPartners
    * New Fulltext Search feature using elasticsearch.
  * [#4239](https://github.com/metasfresh/metasfresh/issues/4239) Be robust wrt priceentered with too many digits
    * Improves the behavior of Priceentrered in documents, depending on Pricelist Price Precisions.
  * [#4240](https://github.com/metasfresh/metasfresh/issues/4240) Translate new Repack Attributes
    * Improved Translation for Repack No. Attributes.
  * [#4242](https://github.com/metasfresh/metasfresh/issues/4242) WebUI: Window Event Log
    * New Window event log added to WebUI Menu.
  * [#4244](https://github.com/metasfresh/metasfresh/issues/4244) Purchase Candidates adjustments
    * Window Improvements for Purchase Candidates in WebUI.
  * [#4146](https://github.com/metasfresh/metasfresh/issues/4146) Picking: Show HU Products with not exact Attribute matching
    * New Feature for Picking in WebUI, now also able to show Handling Units without perfect Attribute Matching.
  * [#4260](https://github.com/metasfresh/metasfresh/issues/4260) Appserver needs to tell SwingUI where to find RabbitMQ
    * Feature to let the App Server know where to find RabbitMQ.
  * [#4264](https://github.com/metasfresh/metasfresh/issues/4264) Ingredients Data for Consumer Product Label
    * New Fields for Consumer Label Ingredients in BOM Line.
  * [#4265](https://github.com/metasfresh/metasfresh/issues/4265) New Window/ Tab for Product Nutrition facts
    * New Windows in WebUI for Nutrition and Product Nutrition maintenance.

## Fixes
* metasfresh
  * [#4255](https://github.com/metasfresh/metasfresh/issues/4255) Contract Person in Charge not filtered by Systemuser
    * Fixed User in Charge Validation,. Now only showing Systemusers/ -contacts in the dropdown selection.
  * [#4266](https://github.com/metasfresh/metasfresh/issues/4266) user notifications are stuck in the event framework
    * Fix for User Notifications, improving the duration between Notification trigger and delivery.
  * [#4268](https://github.com/metasfresh/metasfresh/issues/4268) contract status is set back to running after termination in some unknown cases
    * Fixes issue in contract, having the status set back to running after termination.
  * [#4269](https://github.com/metasfresh/metasfresh/issues/4269) Can't open custom forms in swing anymore
    * Fixes a Bug in Custom Forms. Now possible to open them again in Swing Client.

* metasfresh-webui-frontend
  * [#1811](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1811) Fields are set on null when you press tab too fast
    * Fix for Tab Hold in Document windows. Now not blurring the Fields content anymore when values are already set.
  * [#1837](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1837) Cancel request message disappears too fast
    * Fixes the cancel request message. Now not dissappearing anymore when hovering.
  * [#1843](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1843) Action button not properly displayed in Transportation Order window
    * Fixes the Button Look&Feel in Case the Button has no data from API.
  * [#1853](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1853) Searching in BPartner field from order is not working
    * Improvement of new Businesspartner and search in Order Window.


# metasfresh 5.62 (2018-25)
## Features
* metasfresh
  * [#3028](https://github.com/metasfresh/metasfresh/issues/3028) WebUI: New Window for Import COA
    * New Window Import Chart of Accounts in WebUI.
  * [#4201](https://github.com/metasfresh/metasfresh/issues/4201) WebUI: Show DeliveryRule in Businesspartner Customer and Sales Order
    * Improvement of Businesspartner and Sales Order Window in WebUI. Adding the Field for Delivery Rule.
  * [#4231](https://github.com/metasfresh/metasfresh/issues/4231) Address swing-client performance problem in rechnungsdispo summary info
    * Improving the Performance of Invoice candidates summary info.
  * [#4230](https://github.com/metasfresh/metasfresh/issues/4230) Filter for POReference in Invoicecand
    * Improving the filtering Performance for POReference in Invoice candidates window.
  * [#4153](https://github.com/metasfresh/metasfresh/issues/4153) Serial Letter Feature
    * New Feature allowing to create Serial Letters.

* metasfresh-webui-frontend
  * [#1417](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1417) Shortcuts for delete modal window
    * Improved shortcut Handling in delete record modal overlay.
  * [#1686](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1686) API login for cypress
    * New Feature for Testing Framework Cypress, now allowing the API to do a login.

## Fixes
* metasfresh
  * [#4134](https://github.com/metasfresh/metasfresh/issues/4134) Updating record to not match tab where clause leads to error when PKs are different
    * Fixes a Bug that surfaced after using the new Virtual Tab Feature, causing an Error in where clause with different Primary Keys.
  * [#4232](https://github.com/metasfresh/metasfresh/issues/4232) CleverReach remote group id not stored when campaign is created
    * Bugfix for the CleverReach Feature, now storinf the Remote Group Identifier after creating a new campaign.
  * [#4233](https://github.com/metasfresh/metasfresh/issues/4233) Attributeset as Sysadmin cannot be created
    * Fixes the recording of Attributeset with System Client.

* metasfresh-webui-frontend
  * [#1446](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1446) Tab in purchase order batch entry not working correctly
    * Fixes the Tab usage in Batch entry after confirming selection with mouse.
  * [#1774](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1774) Cannot stop uploading a file
    * Extend File Upload Feature, now possible to cancel the upload.
  * [#1840](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1840) 404 error shall be centered
    * Fixes the 404 error message. Now centered in WebUI Layout.

# metasfresh 5.61 (2018-24)
## Features
* metasfresh
  * [#2539](https://github.com/metasfresh/metasfresh/issues/2539) Translate report_en_US.properties for order, inout, invoice
    * Improvement of report properties Translations for en_US language
  * [#4107](https://github.com/metasfresh/metasfresh/issues/4107) Customer Revenue Report Excel with Credit Limit
    * New Customer Revenue Report as Excel Sheet Download.
  * [#4141](https://github.com/metasfresh/metasfresh/issues/4141) WebUI: Translation Window for Currencies
    * New Window in WebUI that allows to maintain the Currency Translations.
  * [#4142](https://github.com/metasfresh/metasfresh/issues/4142) WebUI: Translation Window for Document Types
    * New Window in WebUI that allows to maintain the Document Type Translations.
  * [#4143](https://github.com/metasfresh/metasfresh/issues/4143) WebUI: Translation Window for Messages
    * New Window in WebUI that allows to maintain the message Translations.
  * [#4151](https://github.com/metasfresh/metasfresh/issues/4151) Import: extend process of importing vendors
    * Improved Vendor importing action, allowing to import a lot of additional infomration for a vendor.
  * [#4167](https://github.com/metasfresh/metasfresh/issues/4167) Process C_Flatrate_Term_Extend shall continue if individual terms fail
    * Improved Flatrate Term extension Action, now proceeding the process even if individual Terms fail.
  * [#4169](https://github.com/metasfresh/metasfresh/issues/4169) Pricing Conditions Jasper
    * New Report that shows the recorded Pricing Conditions per Customer/ Vendor.
  * [#4173](https://github.com/metasfresh/metasfresh/issues/4173) Translations for Purchase Dispo modal Overlay Fields
    * Field Translations added for Purchase Dispo modal overlay in Sales Order and Purchase Candidates.
  * [#4178](https://github.com/metasfresh/metasfresh/issues/4178) Pricing Conditions Cockpit Translations in Material Cockpit
    * Improving Translations for en_US and de_DE for Pricing Conditions Actions.

## Fixes
* metasfresh
  * [#4012](https://github.com/metasfresh/metasfresh/issues/4012) Lot No control in Receipt not working
    * Fixes the Lot No. control in Receipt.
  * [#4168](https://github.com/metasfresh/metasfresh/issues/4168) Error when posting payment allocation with tax correction and multiple taxes
    * Bugfix for the payment allocation posting, wen having a tx correction with multiple taxes.
  * [#4191](https://github.com/metasfresh/metasfresh/issues/4191) Cannot add a product in order
    * Bugfix for the product batcentry in webui, not allowing to add a product in minor cases.
  * [#4149](https://github.com/metasfresh/metasfresh/issues/4149) User query: IUserQueryRestriction is not built properly all the time
    * Fix for the User Query Restriction.

* metasfresh-webui-frontend
  * [#1266](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1266) Labels widget: tab and shift-tab support
    * Improves the usage of Tab and shift-tab for Label widgets.
  * [#1616](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1616) Reload /i18n/messages in case the language changed
    * Improving the language loading of static messages for users with different language than default.
  * [#1617](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1617) Label component doesn't hide after clicking tab
    * Improvement of Tab behavior in label widget when dropdown list is openend. Now closing the Dropdown.
  * [#1808](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1808) Shortcuts for inbox, menu and sidelist
    * Improvement of Shortcuts for inbox, menu and sidelist. Now hiding the menus after 2nd usage of shortcut.
  * [#1820](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1820) Make sure frontend is connecting to view's websocket endpoint BEFORE view data it's fetched
    * Fix for the connection to the websocket endpoint.
  * [#1828](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1828) Truncate action names with ellipsis
    * Fixes the Layout for Quickaction Buttons with large content.
  * [#1830](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1830) Empty login page after logout
    * Fixes the empty page after logout. Now showing the login screen again.
  * [#1832](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1832) Labels widget: pressing enter
    * Improvement of the Pre-Selection of Label Widget Dropdown after Label selection.


# metasfresh 5.60 (2018-23)
## Features
* metasfresh
  * [#4033](https://github.com/metasfresh/metasfresh/issues/4033) Pharma: MSV3 Purchase Functionality in purchase candidates
    * New Feature in Purchase Candidates, now allowing to use the MSV3 Order Functionality there too.
  * [#4116](https://github.com/metasfresh/metasfresh/issues/4116) WebUI: Translation Window for Tax Rates
    * New Window in WebUI for the maintenance of Tax Rate Translations.
  * [#4117](https://github.com/metasfresh/metasfresh/issues/4117) WebUI: Add missing Translations in Product Window
    * Improved the Translations for en_US in Product Window.
  * [#4118](https://github.com/metasfresh/metasfresh/issues/4118) WebUI: Translation Window for Unit of Measures
    * New Window in WebUI for the maintenance of Unit of measure Translations.
  * [#4119](https://github.com/metasfresh/metasfresh/issues/4119) WebUI: Translation Window for Tax Category
    * New Window in WebUI for the maintenance of Tax Category Translations.
  * [#4127](https://github.com/metasfresh/metasfresh/issues/4127) Batch entry product ID
    * Batch Entry improvement, now integrating the Product Identifier configuration.
  * [#4135](https://github.com/metasfresh/metasfresh/issues/4135) Webui: Add Document References to all Windows with Translations
    * Improved the navigation beween master data and translation windows, adding references to the translation window & table.
  * [#4138](https://github.com/metasfresh/metasfresh/issues/4138) WebUI: Translation Window for Paymentterm
    * New Window in WebUI for the maintenance of Payment Term Translations.
  * [#4139](https://github.com/metasfresh/metasfresh/issues/4139) WebUI: Translation Window for Dunning Level
    * New Window in WebUI for the maintenance of Dunning Level Translations.
  * [#4158](https://github.com/metasfresh/metasfresh/issues/4158) WebUI Sitemap: Missing Translations en_US
    * Improvement of the Translation for en_US for the WebUI menu, windows and tabs.
  * [#4161](https://github.com/metasfresh/metasfresh/issues/4161) Improve error message regarding illegal HU status changes
    * Extended error Message for the Notification of invalid Handling Unit State changes.
  * [#4165](https://github.com/metasfresh/metasfresh/issues/4165) Extend Billing Candidates Filtering for contracts
    * New Filter criteria added to billing candidates window, allowing to filter by candidate controller.
  
* metasfresh-webui-frontend
  * [#1311](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1311) Clear Browser Cache when new webui frontend version is installed
    * Improved cache clearing after rollout of new frontend version.

* metasfresh-dist
  * [#45](https://github.com/metasfresh/metasfresh-dist/issues/45) publish standalone jasper/reporting files
    * Internal housekeeping improvement for the automatic publishing of standalone Jasper Files.

## Fixes
* metasfresh
  * [#4122](https://github.com/metasfresh/metasfresh/issues/4122) Transform action throws error
    * Fixes an error in certain cases of Handling Unit Transformations.
  * [#4123](https://github.com/metasfresh/metasfresh/issues/4123) Dunning Jasper does not work
    * Fixes the Jasper Report for Dunning Documents.
  * [#4125](https://github.com/metasfresh/metasfresh/issues/4125) Sometimes I got NPE when posting an allocation
    * Improvement of the Payment Allocation accounting.
  * [#4147](https://github.com/metasfresh/metasfresh/issues/4147) Error when posting a zero-sum invoice
    * Fixes the posting of Invoices with 0 Sum.
  * [#4163](https://github.com/metasfresh/metasfresh/issues/4163) "Overlapping term" error when completing subscription order
    * Fixes an error for the contract creation that occurred when completing a subscription order.

* metasfresh-frontent-webui
  * [#1813](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1813) Cannot set attribute in orderline grid view
    * Fixes the setting of Attributes in Orderline Grid View.
  * [#1814](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1814) Action button is too large
    * Fixes the Layout of Action Button being too large. Also hiding the Action Buttons from Batch Entry again.


# metasfresh 5.59 (2018-22)

**release for week 2018-22**

## Features
* metasfresh
  * [#3263](https://github.com/metasfresh/metasfresh/issues/3263) WebUI: Translation Window for Bill of Materials and Formula
    * New Translation Window in WebUI for Bill of Materials and Formula.
  * [#3307](https://github.com/metasfresh/metasfresh/issues/3307) Order/Invoice jasper: always use the Description/DescriptionBottom from document and don't check C_DocType's description
    * Improving the Order Jasper Documents for Description bottom information.
  * [#3323](https://github.com/metasfresh/metasfresh/issues/3323) WebUI Window Design: Improve window Rechnungskandidaten - Handler
    * Improved Invoicecandidate Handler Window in WebUI.
  * [#3996](https://github.com/metasfresh/metasfresh/issues/3996) WebUI: Client window: EMail fields layout
    * Improved Client Window in WebUI. Grouping eMail Fields and new Translations for de_DE Language.
  * [#4000](https://github.com/metasfresh/metasfresh/issues/4000) New Report for Yearly Bonus
    * New Report that shows the Invoice Candidates for Yearly Bonus Contracts that can be invoiced.
  * [#4015](https://github.com/metasfresh/metasfresh/issues/4015) CleverReach Interface
    * New Feature that adds Cleverreach eMail Marketing functionalities.
  * [#4031](https://github.com/metasfresh/metasfresh/issues/4031) Add easy way to add AD_Users to Newsletter marketing campaigns
    * New Feature that allows to add Users to the new Newsletter marketing campaign feature.
  * [#4035](https://github.com/metasfresh/metasfresh/issues/4035) Proforma Invoice via Sales Order workflow
    * New Documenttype for Proforma Invoices, implementted as Sales Order Documenttype and added into shipment candidates/ invoice candidates workflow.
  * [#4036](https://github.com/metasfresh/metasfresh/issues/4036) Sales Order: Show Pricing Conditions in create purchase order action
    * Extended modal overlay of create purchase order action, now showing advanced information about vendor pricing conditions.
  * [#4042](https://github.com/metasfresh/metasfresh/issues/4042) Pharma: extend customer import 
    * Extended the customer Import functionality.
  * [#4058](https://github.com/metasfresh/metasfresh/issues/4058) Add delivery times to Der Kurier
    * Extended the Implementation of the "Der Kurier" Logistics provider. Now adding the delivery/ fetching times.
  * [#4083](https://github.com/metasfresh/metasfresh/issues/4083) Make refund contract doctypes
    * New Document Types - Refund Invoice, Refund Credit Memo - for the Yearly Refund Contracts.
  * [#4085](https://github.com/metasfresh/metasfresh/issues/4085) Create relation from candidate to refund-candidate
    * New Document reference added for the relation between regular invoice candidate and refund invoice candidate.
  * [#4089](https://github.com/metasfresh/metasfresh/issues/4089) Create missing fields for Bonus in WebUI
    * New Fields added to Purchase Orderline and Invoice Candidate for Refund Contracts.
  * [#4094](https://github.com/metasfresh/metasfresh/issues/4094) Create Mandatory Logic in Contract terms
    * Improved Window for contract terms, now having a mandatory Logic for fields not needed for Refund Contract Types.
  * [#4096](https://github.com/metasfresh/metasfresh/issues/4096) User Queries : turn list fields for table and tab into search fields
    * Improving Filtering of User Queries in WebUI.
  * [#4102](https://github.com/metasfresh/metasfresh/issues/4102) Webui: Purchase schedule tab - trl and display
    * Improved Purchase Schedule Subtab in WebUI. New Translations added.

## Fixes
* metasfresh
  * [#3463](https://github.com/metasfresh/metasfresh/issues/3463) "Issue only for what was received" not working anymore
    * Fixes a Bug in Issue Method "Issue only what was received", now allowing to isse the exactly planned quantity again.
  * [#4078](https://github.com/metasfresh/metasfresh/issues/4078) AD_User_ID/Bill_User_ID not set in Sales Order when using Quick creation of partner
    * Fixes a Bug in Sales Order Contact. Now setting the User and Bill User also when creating a new Business Partner on the Fly.
  * [#4079](https://github.com/metasfresh/metasfresh/issues/4079) Contact is not set when order is cloned
    * Improvement of the Close Feature of Sales Order. The Contact is now also copied.
  * [#4087](https://github.com/metasfresh/metasfresh/issues/4087) Credit limit with different bill BPartner
    * Improvement of the Credit Limit check in Sales Order, now checking agaist the Billto Businesspartner Credit Limit.

* metasfresh-webui-frontend
  * [#1717](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1717) Date Format in date range picker is not localized
    * Fixes the Localization of Dates in Date Range Picker Widget.
  * [#1794](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1794) Modal view editing issues
    * Fixes issues in modal view field editing.
  * [#1800](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1800) Material Receipt Candidate: first line is not pre-selected and no action button available when opening HU Editor
    * Improvement of the Quickaction handling of preselected first lines when opening a window initially.
  * [#1801](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1801) Error when opening HU Editor window / selecting a HU in picking tray clearing
    * Fixes a number format exception in handling Unit Editor window.
  * [#1805](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1805) Multi Line Text fields are displayed infinitely
    * Now restricting the length of Multiline Text fields in Data Grids.

# metasfresh 5.58 (2018-21)

**release for week 2018-21**

## Features
* metasfresh
  * [#3753](https://github.com/metasfresh/metasfresh/issues/3753) Inventory: Prepare Inventorylines shall update existing lines
    * Improvement of the Inventory Prepare Action, now updateing existing lines instead of creating new ones.
  * [#3879](https://github.com/metasfresh/metasfresh/issues/3879) Add link and templates for email notification
    * New Feature in eMail Notifications, now allowing to add Links and using Mail Templates.
  * [#3999](https://github.com/metasfresh/metasfresh/issues/3999) New contract Type: Yearly Bonus from vendors
    * New Contract Type for vendors "Refund Bonus".
  * [#4001](https://github.com/metasfresh/metasfresh/issues/4001) Calculate Purchase price with yearly Bonus
    * Calculating of Purchase Cost Prices now also reflecting the new Contract Type Terms for "Refund Bonus".
  * [#4002](https://github.com/metasfresh/metasfresh/issues/4002) Purchase Order Aggregation
    * New Functionality for Purchase Order Aggregations. Allowing to set lead times for Vendors and latest Purchasing times per Day. When date and time is reached, then Notification can be sent to notification Group. The Purchase Order candidates for the vendor are then automatically aggregated into a Purchase Order.
  * [#4030](https://github.com/metasfresh/metasfresh/issues/4030) Create webui windows for marketing and cleverreach settings
    * New WebUI Windows for the new Marketing Feature of Cleverreach.
  * [#4032](https://github.com/metasfresh/metasfresh/issues/4032) Show Pricing Conditions of Business Partner
    * New Feature in Material Cocpit. Now it's possible to show the Pricing Conditions of Businessparters for a selected Product via Material Cockpit window in WebUI.
  * [#4070](https://github.com/metasfresh/metasfresh/issues/4070) WebUI Windows for new contract Type "Yearly Bonus from vendors"
    * New WebUI Windows for the new Contract Type "Refund Bonus".
  * [#4073](https://github.com/metasfresh/metasfresh/issues/4073) Virtual Tabs implementation
    * New Feature in Application Dictionary that allows to define Tabs as Virtual, and then reuse it in multiple windows.
  * [#4047](https://github.com/metasfresh/metasfresh/issues/4047) CleverReach get paginated receivers list
    * Reacting now on maximum allowed Batch sizes when receiving data from Cleverreach.
  * [#4056](https://github.com/metasfresh/metasfresh/issues/4056) webui: pimp Partner Pharma - Purchase schedule tab
    * New Subtab in Pharma Partner Window, now allowing to configure Purchase Schedules for the new Purchase Aggregation Functionality.
  * [#4062](https://github.com/metasfresh/metasfresh/issues/4062) Pricing conditions modal: allow changing pricing type, edit pricing system etc
    * Improved Pricing Conditions overview. Now possible to edit more data in Pricing Conditions modal.
  * [#4071](https://github.com/metasfresh/metasfresh/issues/4071) Exception handling: make them more translatable
    * Improving the Error Handling and Notifications, now showing translateable Error Messages.

* metasfresh-webui-frontend
  * [#1789](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1789) User notifications: handle view target type
    * Improved Handling of User notificaitons in WebUI, now handling the view target type.

* metasfresh-dist
  * [#18](https://github.com/metasfresh/metasfresh-dist/issues/18) Create docker image automatically via jenkins
    * Now automatically creating metasfresh docker images via jenkins and uploading them to dockerhub.

* metasfresh-dist-orgs
  * [#93](https://github.com/metasfresh/metasfresh-dist-orgs/issues/92) Postal Lookup for Switzerland CH
    * Imported and fresh Postal Data for the Postal Lookup in Switzerland.

## Fixes
* metasfresh
  * [#3792](https://github.com/metasfresh/metasfresh/issues/3729) Setting a different invoice bpartner causes error
    * Fixes an Error in Sales Order, that lead to an Exception when selecting a different Invoice Partner.
  * [#4018](https://github.com/metasfresh/metasfresh/issues/4018) QtyCU not respected in Quarantine DD_Orderline
    * Fixes the wrong Quantity in Distribution Orderlines for Movements to Quarantine Warehouse.
  * [#4052](https://github.com/metasfresh/metasfresh/issues/4052) NPE when deleting inoutline with empty product
    * Fixes a Null Pointer Exception when deleting Inout Lines without a Product set.
  * [#4063](https://github.com/metasfresh/metasfresh/issues/4063) Enhanced Pricing: Discount Break is falsely invalidated
    * Improvement of the Enhanced Pricing Rules.

* metasfresh-webui-frontend
  * [#1790](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1790) View: refresh after removing a static filter
    * Improvement in WebUI Frontend, now refreshing the view after removing a static filter.

# metasfresh 5.57 (2018-20)

**release for week 2018-20**

## Features
* metasfresh
  * [#3754](https://github.com/metasfresh/metasfresh/issues/3754) Inventory: Allow only "Active" and "Issued" HUs in inventorylines
    * Improved Inventory Feature, only allowing active and issued Handling Units in Inventory Lines.
  * [#3975](https://github.com/metasfresh/metasfresh/issues/3975) Allow annotating data as personal
    * New Feature for GDPR Compliance that allows to annotate data as personal Data via Applicaiton Dictionary.
  * [#3991](https://github.com/metasfresh/metasfresh/issues/3991) Implement "Der Kurier" parcel number check digit
    * New Feature creating a check digit for the new Logistics Provider Implementation of "Der Kurier"
  * [#3993](https://github.com/metasfresh/metasfresh/issues/3993) Eliminate the ampersand from all AD_Messages
    * Improvement for Messaged, eliminating all Ampersand characters.
  * [#4003](https://github.com/metasfresh/metasfresh/issues/4003) Adjust Window "Der Kurier Versandauftrag"
    * New Window for a new Logistics Partner Order window of "Der Kurier".
  * [#4004](https://github.com/metasfresh/metasfresh/issues/4004) WebUI: Adjust new Window Discount Schema Pharma
    * Improved Window for Discount Schema Pharma.
  * [#4029](https://github.com/metasfresh/metasfresh/pull/4029) CleverReach Interface generic marketing datamodel
    * New Implemetation of the CleverReach marketing data model.
  * [#4034](https://github.com/metasfresh/metasfresh/issues/4034) Add CustomerCode and CollectorCode to Der Kurier
    * Additional Implemantation for the new Logistics Provider "Der Kurier"

* metasfresh-webui-frontend
  * [#1613](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1613) Display field changes warnings
    * New Field notification feature. This allow to add user notifications to fields about infos or error messages.
  * [#1624](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1624) Material Cockpit Filter Name + switch date = invalid date
    * Improvement of the Filtering and Navigation in Material Cockpit.

* metasfresh-dist
  * [#41](https://github.com/metasfresh/metasfresh-dist/issues/41) Fix and improvement around picking/shipping
    * Improves the Picking Slot locators for compression workflow.

# Fixes
* metasfresh
  * [#4013](https://github.com/metasfresh/metasfresh/issues/4013) Lot No Action error when running multiple times
    * Fixes the Lot No Action, now allowing to run the Action multiple times without errors.
  * [#4017](https://github.com/metasfresh/metasfresh/issues/4017) Vendor Action for adding (temp.) Pricing Conditions in Purchase Order missing
  * [#4020](https://github.com/metasfresh/metasfresh/issues/4020) eventlog data needs to be stored out-of-trx
    * Internal Housekeeping improvement, now storing eventlog data out of transaction.
  * [#4027](https://github.com/metasfresh/metasfresh/issues/4027) "To Be Updated" in shipment schedule and "In Verarbeitung" in workpackage getting stuck
    * Fixes a Bug about blocked workpackages in workpackage processing for shipment schedule entries.
  * [#3980](https://github.com/metasfresh/metasfresh/issues/3980) Notifications in Swing Client show no info
    * Fixes the Notification feature in Swing Client, now showing detailed information body again.
  * [#4016](https://github.com/metasfresh/metasfresh/issues/4016) Pricing Conditions error when save
    * Fixes an error mit null value in pricing conditions seqno. Now allowing to save the pricing conditions again.
  * [#4028](https://github.com/metasfresh/metasfresh/issues/4028) Multiple shipment lines for one order line all have the order line's TU-Qty
    * Fix for the Transporation Unit Quantity in shipment lines, for multiple shipment lines for one orderline.

* metasfresh-webui-frontend
  * [#1751](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1751) HU Editor: selection jumps from your line to first line
    * Improved behavior of seletion lines in Handling Unit Editor when changing referenced data. Now the selection is not jumping away anymore.
  * [#1765](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1765) Modal view: editing lookups not working
    * Fixes the usage of Lookup widgets in modal Overlays. Now accessing the correct endpoints.
  * [#1784](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1784) Search fields in filters are not working
    * Fixes a Bug in Lookup Filters.

## Fixes

# metasfresh 5.56 (2018-19)

**release for week 2018-19**

## Features
* metasfresh
  * [#3312](https://github.com/metasfresh/metasfresh/issues/3312) Webui Window Design: Improve window Table and Column
    * New Window for Table and columns in WebUI.
  * [#3812](https://github.com/metasfresh/metasfresh/issues/3812) Add process for creating missing M_Product_acct records to WebUI
    * New Action added to Product Catregory window, allowing to copy Acctounting Setting to all Products of a Product Category.
  * [#3926](https://github.com/metasfresh/metasfresh/issues/3926) Implement support for `der Kurier` shipper
    * New Logistic Provider Implementation of "Der Kurier".
  * [#3965](https://github.com/metasfresh/metasfresh/issues/3965) Translate Actions Update Pharma Conditions
    * New Translations for Pharma Condition Parms in Updatte Pharma Permissions Action for de_DE, en_US.
  * [#3967](https://github.com/metasfresh/metasfresh/issues/3967) Translate Process Parm in Update Pharma Conditions for Customers
    * Improved Translations for Action Parms. Languages de_DE, en_US.
  * [#3969](https://github.com/metasfresh/metasfresh/issues/3969) Pharma: If Shipment Auth Type B then show in Order Header
    * New Feature in Sales Order, now showing The Shipment Auth Type if it's Type B.
  * [#3973](https://github.com/metasfresh/metasfresh/issues/3973) Manufacturing Workflow adjustments in WebUI
    * Improved Manufacturing Workflow Window in WebUI.
  * [#3982](https://github.com/metasfresh/metasfresh/issues/3982) Pharma vertical for Discount Schema Window
    * New Window for Discount Schema for Pharma verticals.
  * [#3989](https://github.com/metasfresh/metasfresh/issues/3989) Pharma: repack number attributes
    * New Functionality for Pharma Verticals, allowing to define the need of recording repack No in Material Receipt.

* metasfresh-webui-api
  * [#952](https://github.com/metasfresh/metasfresh-webui-api/issues/952) Shorten the ViewIds
    * New Feature for WebUI that shortens the View IDs.
  * [#954](https://github.com/metasfresh/metasfresh-webui-api/issues/954) Allow configuring lookup cache reset on table record changes
    * Improved cache resetting. Now it's able to configure the caching behavior for lookups on table record changes.

* metasfresh-webui-frontend
  * [#1772](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1772) Harmonize List widget Icon Look&Feel when not empty
    * Improved Look&Feel of List Widgets, now showing only 1 icon depending on field state.

## Fixes
* metasfresh
  * [#2558](https://github.com/metasfresh/metasfresh/issues/2558) All existing configs available in Gebindekonfiguration in PP_Order
    * Fixes the available Picking Instructions in manufacturing Order. Now only showing those which fit for the selected Product.
  * [#3916](https://github.com/metasfresh/metasfresh/issues/3916) QtyPicked not updated in shipment schedule after reactivate & unpick in picking terminal
    * Fixes the Quantity Picked amount after reactivating and unpicking in Picking Terminal.
  * [#3971](https://github.com/metasfresh/metasfresh/issues/3971) New Manufacturing Workflow not saved
    * Adds missing Field to Manufacturing Workflow View in WebUI, allowing to save a workflow record again.
  * [#3977](https://github.com/metasfresh/metasfresh/issues/3977) Pharma: Prices from IFA import are in cents
    * Fixes the Import Format for the IFA Pharma Product Import.
  * [#3984](https://github.com/metasfresh/metasfresh/issues/3984) Invoice candidate for canceled term and reactivated sales order keeps invalidating itself
    * Fixes an infinite loop of recomputes of invoice canidates for cancelled flatrate terms after reactivating sales orders.
  * [#4022](https://github.com/metasfresh/metasfresh/issues/4022) NPE in FlatrateBL.extendContract()
    * Fixes a Null Pointer Exception in Flatrate term contract handling.

* metasfresh-webui-api
  * [#959](https://github.com/metasfresh/metasfresh-webui-api/issues/959) NPE when opening Manufacturing Issue/Receipt
    * Fixes a Null Pointer Exception when opening a Manufacturing Issue or Receipt.

* metasfresh-webui-frontend
  * [#1410](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1410) Shortcuts for Clone & Letter not working
    * Fixes the not working shortcuts for letter and clone.
  * [#1767](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1767) Letter modal throws errors
    * Fixes the modal Letter view.
  * [#1768](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1768) Cloning document throws error
    * Fixes an error that appeared when starting the clone Action via keyboard shortcut instead of mouse.
  * [#1771](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1771) Date Field Content not aligned 1px
    * Improved alignment of Date and Date-Time Field Content.

# metasfresh 5.55 (2018-18)

**release for week 2018-18**

## Features
* metasfresh
  * [#3026](https://github.com/metasfresh/metasfresh/issues/3026) WebUI: New Window for Import Product
    * New Window in WebUI for Import Product.
  * [#3301](https://github.com/metasfresh/metasfresh/issues/3301) Allow Batchbooking via Payment Selection
    * New Feature in Payment Selection Export. Now allowing to use Batchbooking in Sepa Exports.
  * [#3664](https://github.com/metasfresh/metasfresh/issues/3664) WebUI: Add translation for upload notification
    * Improved Translations for the Upload notifications.
  * [#3708](https://github.com/metasfresh/metasfresh/issues/3708) Send Mail too when notification
    * New Feature that allows to configure Notification Setting for a User and receiving an email as notification too.
  * [#3740](https://github.com/metasfresh/metasfresh/issues/3740) WebUI add Warehouse PO column to Organization/Org Info window
    * New Field for Purchase Warehouse added to Orginfo Subtab in Organisation window.
  * [#3800](https://github.com/metasfresh/metasfresh/issues/3800) Improve inventory import
    * Improved Inventory import action.
  * [#3814](https://github.com/metasfresh/metasfresh/issues/3814) WebUI: My Profile: display Notification Type and User In Charge
    * New Fields in myProfile Window that allows detailed Notifications Settings for the user.
  * [#3837](https://github.com/metasfresh/metasfresh/issues/3837) MSV3 products ban list
    * New Feature in Pharma Vertical, allowing to use Product Ban lists that decide if Products shall be offered to a customer via MSV3 Server or not.
  * [#3839](https://github.com/metasfresh/metasfresh/issues/3839) WebUI: BPartner window: show BPartner Product tab
    * Improvement of Business Partner window. Now allowing to record Products that shall not be sold to a specific BPartner.
  * [#3869](https://github.com/metasfresh/metasfresh/issues/3869) Procurement - add AD_Issue_ID to I_PMM_QtyReport_Event, I_PMM_WeekReport_Event and I_PMM_RfQResponse_ChangeEvent
    * Improvement of the Issue Handling in Procurement Report Events.
  * [#3875](https://github.com/metasfresh/metasfresh/issues/3875) Request notifications shall use new notifications API
    * Improving the creation of Request notifications, now using the new Notification API.
  * [#3889](https://github.com/metasfresh/metasfresh/issues/3889) Report for Pharma Permission/ Authorisation control
    * New Report for Pharma Verticals that shows the Authorisation certificates of customers/ vendors.
  * [#3891](https://github.com/metasfresh/metasfresh/issues/3891) Pharma: Don't allow recording of pricing conditions that are not allowed
    * Improved Pricing recording for Pharma Verticals, restricting not allowed pricing conditions.
  * [#3899](https://github.com/metasfresh/metasfresh/issues/3899) Webui window for M_HU_Process
    * New Window for the Configuration of Handling Unit Processes. Can be used as System Administrator.
  * [#3909](https://github.com/metasfresh/metasfresh/issues/3909) Docoutbound mailing: Autodect if MailWorkpackageProcessor.EmailMessage is HTML
    * Improved Document Outbounf Feature, now allowing to configure and use formatted HTML Mails instead of plain text.
  * [#3910](https://github.com/metasfresh/metasfresh/issues/3910) Credit limit: treat credit status on NULL as it would be X (No check)
    * Credit Status improvement, now handling null values as no credit check.
  * [#3914](https://github.com/metasfresh/metasfresh/issues/3914) Avoid numeric values with too many trailing zeros
    * Improved number handling fith trailing digits, voiding too many zeroes.
  * [#3917](https://github.com/metasfresh/metasfresh/issues/3917) Fail on complete for order lines with no pricing conditions
    * New Pricing feature in sales order, failing to complete/ record lines withour recorded pricing conditions.
  * [#3925](https://github.com/metasfresh/metasfresh/issues/3925) Sales order: just-in-time creation of conditions for a product without conditions
    * New Feature in Sales Order, allowing to record pricing conditions on the fly.
  * [#3929](https://github.com/metasfresh/metasfresh/issues/3929) Show BasePriceSystem in Document Line and Documents
    * Improved document lines, now showing the Base Price System from Pricing Conditions.
  * [#3937](https://github.com/metasfresh/metasfresh/issues/3937) Create process for importing discount schema
    * New Process that allows to import discount schema data.
  * [#3945](https://github.com/metasfresh/metasfresh/issues/3945) Get rid of "QtyReserverd Recalculate" AD_Scheduler_ID=550010
    * Housekeeping Issue, getting rid of legacy scheduled Process.
  * [#3946](https://github.com/metasfresh/metasfresh/issues/3946) Write M_ShipmentScheduleRecompute.AD_Pinstance_ID to queue-wp-log
    * Housekeeping Issue, now logging the Process Instance to the workpackage log.
  * [#3960](https://github.com/metasfresh/metasfresh/issues/3960) Improve the speed of scripts applier
    * Improved the scripts applier, reducing the runtime of migration scripts check by 80%.

* metasfresh-webui-api
  * [#956](https://github.com/metasfresh/metasfresh-webui-api/issues/956) Rest endpoint: delete all notifications
    * New endpoint that allows to delete all notifications at once.

* metasfresh-webui-frontend
  * [#1603](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1603) Color Indicator Widget functionality
    * New Color presentation Widget.

## Fixes
* metasfresh
  * [#3847](https://github.com/metasfresh/metasfresh/issues/3847) Migration script not logged for creating new ad_ui_section when value is not manually filled
    * Bugfix for WebUI Window cration and migration, now not leaving a broken migration script when not filling the value of a UI Section.
  * [#3880](https://github.com/metasfresh/metasfresh/issues/3880) ShipmentLines's TU-Qty is updated wrongly from schedule's QtyOrdered_Override
    * Fixes a Bug in Shipment Schedule, now updateing the TU Quantity correctly.
  * [#3923](https://github.com/metasfresh/metasfresh/issues/3923) Change Picking Terminal columns and fix auto process picking
    * Fixes a Bug in Picking Window in WebUI, now showing Quantity Picked instead of Quanitity picked planned, and further improvements.
  * [#3927](https://github.com/metasfresh/metasfresh/issues/3927) Base Price + Surplus in Pricing Conditions not working
    * Bugfix for the new Pricing Rule with Base Prive and Surplus calculation.
  * [#3928](https://github.com/metasfresh/metasfresh/issues/3928) Picking: Reactivate Picked HU/ Processed Picking
    * Fixes an Exception in Picking Window thrown when reactivating processed Pickings.
  * [#3933](https://github.com/metasfresh/metasfresh/issues/3933) Credit limit: Credit used does not update when you reverse/void order
    * Credit Limit fix, now recaclulating the credit used amount when reversing or voiding an order.
  * [#3935](https://github.com/metasfresh/metasfresh/issues/3935) Material Dispo wrong Quantities after Material receipt
    * Fixes the Avialable to Promise quantity after Material Receipt.
  * [#3981](https://github.com/metasfresh/metasfresh/issues/3981) QtyPicked remains set although shipment is completed
  * [#3986](https://github.com/metasfresh/metasfresh/issues/3986) QtyPicked in Picking Terminal set to 0 after partial shipment completed

* metasfresh-webui-api
  * [#945](https://github.com/metasfresh/metasfresh-webui-api/issues/945) Business Partner Pharma Product Create New Issue
    * Fixes an error when creating Business Partner Product entries in Pharma Business Partner window.
  * [#949](https://github.com/metasfresh/metasfresh-webui-api/issues/949) Business Partner Pharma Product Org
    * Bugfix in Business Partner Pharma Window. Now setting the correct Organisation when creating a new Business Partner Product record.

* metasfresh-webui-frontend
  * [#1540](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1540) Shortcut Alt++ not working on non German Keyboard Layout
    * Fixes shortcuts for expand action in WebUI.
  * [#1748](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1748) X not available for field invoice partner when first setting the partner in order
    * Fixes the bahavior of Lookup Combos whe using the clear button.
  * [#1752](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1752) Shortcuts not working on Mac
    * Fixes the Shortcuts for Mac Users.
  * [#1755](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1755) Date field does not recognize changes on double click
    * Fixes the selection and save of date fields when double-clicking on date in date widget.
  * [#1756](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1756) [alt]++ and [alt]+q not working properly anymore
    * Fixes issues about the shortcut handling in WebUI.
  * [#1759](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1759) Enter not working for selecting a role when logging in
    * Fixes the keyboard Handling in Login Role Selection View. Now it's possible to use ENTER for Role selection confirmation.
  

# metasfresh 5.54 (2018-17)
**release for week 2018-17**

## Features
* metasfresh
  * [#3478](https://github.com/metasfresh/metasfresh/issues/3478) Window design: product Pharma
    * Improved Window Layout and Translation for Product Pharma.
  * [#3479](https://github.com/metasfresh/metasfresh/issues/3479) Window design: Business Partner Pharma
    * Improved Window Layout and Translation for Business Partner Pharma.
  * [#3763](https://github.com/metasfresh/metasfresh/issues/3763) Contracts: Create a function that provides a hierarchy of contracts
    * New function that allows to retrieve the hierarchy of created contracts.
  * [#3768](https://github.com/metasfresh/metasfresh/issues/3768) Excel Report for vendor assessment
    * New Excel Report that allows the assessment of vendors.
  * [#3777](https://github.com/metasfresh/metasfresh/issues/3777) Show available to promise in Procurement Dispo modal in Sales Order
    * Improvement of the Procurement Dispo modal overlay, now showing the Available to Promise Quantity.
  * [#3827](https://github.com/metasfresh/metasfresh/issues/3827) Support SSL / TLS when sending mails via SMTP making it SMTPS
    * Improved Mail handling, now allowing the support of SSL/ TLS Handshakes when sending emails.
  * [#3834](https://github.com/metasfresh/metasfresh/issues/3834) Check if Product is banned in Batch entry/ Document Lines creation
    * New Functionality in Sales and Purchase Order. It's now possible to put Products on Ban Lists for customers and vendors. Although the products remain on general Product Price Lists, the products are then prohibited to be recorded. The user gets informed why the product is banned for a specific Business Partner.
  * [#3866](https://github.com/metasfresh/metasfresh/issues/3866) WebUI: Translation for Product LotNo Lock Window
    * Improved Window Layout and additional Translations for de_DE and en_US.
  * [#3873](https://github.com/metasfresh/metasfresh/issues/3873) Performance problem on reactivating large shipment
    * Performance Improvement on reactivation of large shipment documents.
  * [#3887](https://github.com/metasfresh/metasfresh/issues/3887) Automatic Setting of Pharma Authorisation for Shipment/ Receipt
    * New Functionality in Business Partner Pharma window, now settign the Shipment and Receipt Authorisation automatically as soon as the recording of different Permission Types have been done.
  * [#3888](https://github.com/metasfresh/metasfresh/issues/3888) Pharma Business Partner Window adjustments
    * Extended Business Partner Window for Pharma verticals. New Fields that describe the Pharma Trading Permissions of customers and vendors.
  * [#3890](https://github.com/metasfresh/metasfresh/issues/3890) Role Permission for Pharma Permission and Authorization changes
    * New Functionality for Pharma Business Partner that allows to restrict the actions for permission adjustments to specific users and roles.
  * [#3892](https://github.com/metasfresh/metasfresh/issues/3892) Contracts: Allow possibility to copy the prices when extending
    * Improvement of contracts extending, now allowing to copy the prices from the source/ initial contract.
  * [#3895](https://github.com/metasfresh/metasfresh/issues/3895) Extend M_HU_Process
    * New Feature that decouples actions in M_HU_Processn from the presentation in Action menu. Now allowing to hide actions in menu.
  * [#3897](https://github.com/metasfresh/metasfresh/issues/3897) Add Translations for Pharma Business Partner Window
    * New Translations for de_DE and en_US added to Business Partner Pharma Window.

# metasfresh-docker
  * [#34](https://github.com/metasfresh/metasfresh-docker/issues/34) Add msv3server to metasfresh-docker as "extras"
    * Now the Pharma Customer Server is available in metasfresh-docker for MSV3 Communication.

## Fixes
* metasfresh
  * [#3797](https://github.com/metasfresh/metasfresh/issues/3797) Error in BOM Lines for Packaging Component Type and Variant Groups
    * Fixes the error when defining Packaging Component Variants in BOM Lines.
  * [#3859](https://github.com/metasfresh/metasfresh/issues/3859) Credit Limit: Prioritize by date and then seq No from Credit Limit type
    * Improved priotization of Credit Limit Configuration Lines.
  * [#3861](https://github.com/metasfresh/metasfresh/issues/3861) StockChangedEvent can't be serialized
    * Internal Housekeeping. Now allowing the serialization of the StockChangeEvent.
  * [#3863](https://github.com/metasfresh/metasfresh/issues/3863) Missing migration of C_BPartner_Stats.SOCreditStatus on some systems
    * Fixes a Bug around missing Migrations of the Credit Status.
  * [#3864](https://github.com/metasfresh/metasfresh/issues/3864) C_FlatrateTerm.C_Currency is not forwarded when a flatrateTerm is extended
    * Fixes a Bug in Flatrate Term extension, now forwarding the Currency too.
  * [#3876](https://github.com/metasfresh/metasfresh/issues/3876) Different issues around invoice candidate updating
    * Fixes various issues in invoice candidate recompute/ update process.
  * [#3883](https://github.com/metasfresh/metasfresh/issues/3883) Cannot import products
    * Bugfix for the failing product impiort because of a missing isDefault column in Tax Category.
  * [#3885](https://github.com/metasfresh/metasfresh/issues/3885) Process C_Flatrate_Term_Extend does not work if ContractStatus is null
    * Fixes a Bug in the Flatrate term extension process when Contract Status is null.
  * [#3894](https://github.com/metasfresh/metasfresh/issues/3894) NPE on sales order complete
    * Fixes a Null Pointer Exception in Sales Order complete Document Action.

# metasfresh 5.53 (2018-16)
**release for week 2018-16**

## Features
* metasfresh
  * [#3816](https://github.com/metasfresh/metasfresh/issues/3816) Technical: Adapt Query.list() to avoid ClassCastExceptions
    * Internal development issue, improving the Query.list() method to avoid Class Cast exceptions.
  * [#3833](https://github.com/metasfresh/metasfresh/issues/3833) Enhanced Pricing, allowing detailed individual Pricesystems per Product and Business Partner
    * Improved Pricing Calculation functionality, now allowing to overwrite the general Pricing System via Pricing Conditions Schema and Product.
  * [#3835](https://github.com/metasfresh/metasfresh/issues/3835) No recording of Products without pricing Conditions
    * Restriction Functionality, allowing prohibit the recording of Products in Document Lines without individual Pricing conditions.
  * [#3844](https://github.com/metasfresh/metasfresh/issues/3844) WebUI: Add Translations for Context Menu to de_DE
    * Adds new Translations for context menu of metasfresh WebUI.
  * [#3849](https://github.com/metasfresh/metasfresh/issues/3849) Error with ATP presentation in Sales Order Batch entry
    * Fixes a Bug in Sales Order Line Batch entry. Now showing the ATP value in Product Lookup Batch List when configured.

* metasfresh-webui-api
  * [#852](https://github.com/metasfresh/metasfresh-webui-api/issues/852) Color Indicator Widget functionality API
    * New API for color Indicators. This will be used by a new color indicator widget in WebUI frontend soon.

* metasfresh-webui-frontend
  * [#1539](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1539) eMail Editor mailTo List not showing selected entry
    * Improvement of the Adress Lookup in eMail Editor. Now showing which entry is selected.
  * [#1648](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1648) Dropdown value in filters cannot be deleted after selection
    * Improvement of Filter ctiteria, now possible to empty already set values in List Widgets.
  * [#1742](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1742) Context Menu translateable
    * Improvement of Context Menu in Grid View, now translatable.

## Fixes
* metasfresh
  * [#3375](https://github.com/metasfresh/metasfresh/issues/3375) Quantity picked in Shipment Schedules doesn't update
    * Fixes a Bug in Shipment Schedule that prevented the update of Quantity Picked.
  * [#3819](https://github.com/metasfresh/metasfresh/issues/3819) EDI - "Resubmit Selection" from import processor log not working anymore
    * Fixes the action resubmit selection in EDI Import processor log.
  * [#3822](https://github.com/metasfresh/metasfresh/issues/3822) ShipmentSchedule.QtyPickList not updated from drafted shipments
    * Fixes an Error that prevented the update of Shipment Schedule entries for drafted Shipmentlines.
  * [#3838](https://github.com/metasfresh/metasfresh/issues/3838) Packaging invoice candidate updated incorrectly
    * Fixes a Bug in Invoice Candidates that created w wrong update for lines which with packaging material products.
  * [#3842](https://github.com/metasfresh/metasfresh/issues/3842) Cannot access server logs via Server Monitor
    * Internal services and maintenance issue. Now it's possible to access the logs via Server Monitor again.
  * [#3843](https://github.com/metasfresh/metasfresh/issues/3843) Wrong parent.relativePath in different pom.xmls
    * thx to [#gp1864](https://github.com/gp1864)!

* metasfresh-webui-api
  * [#902](https://github.com/metasfresh/metasfresh-webui-api/issues/902) API token is not shown in the webui
    * Improved User Window with Authentication Subtab.
  
* metasfresh-webui-frontend
  * [#1274](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1274) Edit Fields in Main Grid View Improvements
    * Minor Improvement of Grid Cell Edit Mode, now aboiding the Detail View if double Clicking on Field in Edit Mode.
  * [#1462](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1462) Broke: cannot completely delete a numeric field in grid view
    * Fixes the Grid View Edit Mode for numeric Fields that shall be zeroed when backspace.
  * [#1612](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1612) Modal view: quickActions not called when selecting all rows from all pages
    * Fixes the possibility to select more than 20 Grid lines and use Quickactions.

# metasfresh 5.52 (2018-15)
**release for week 2018-15**

## Features
* metasfresh-webui-frontend
  * [#1709](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1709) Harmonize Border Look&Feel between Lookup and List widget
    * Improvement of List widget border to Lookup widget border. Now having a harmonized look & feel.

## Fixes
* metasfresh
  * [#3767](https://github.com/metasfresh/metasfresh/issues/3767) Picking TU Label error when GLN is missing in PartnerLocation
    * Fixes an error in the Picking Label. Now hiding the Barcode in case the Businesspartner does not have a GLN.
  * [#3773](https://github.com/metasfresh/metasfresh/issues/3773) Regression on process M_ReceiptSchedule_Generate_M_InOuts
    * Fixes various issues in the Receipt Document generation Process in Material Receipt Schedule.
  * [#3806](https://github.com/metasfresh/metasfresh/issues/3806) Packaging-inout-lines are split into too many invoice candidates
    * Fixes an error in Invoice Generation with not grouping Packaging Lines in Invoice Candidates.
  * [#3809](https://github.com/metasfresh/metasfresh/issues/3809) InvoiceCandidates without C_PaymentTerm_ID can't be invoiced together with other ICs
    * Fixes an Error in Invoice Candidates. The Packaging Inoutlines had a wrong PaymentTerm and were not grouped/ matched be the new Aggregation Header.
  * [#3815](https://github.com/metasfresh/metasfresh/issues/3815) QtyOrdered sometimes updated wrongly on C_Order close
    * Bugfix for the Quantity Ordered result in Invoicecandidates, that was wrongly set after creation and immediate close of sales orders.

* metasfresh-webui-frontend
  * [#1555](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1555) Can not enter "-" into any search field
    * Fixes the search and filtering for special characters. Now it's able to search for minus, underscore and different other characters too.
  * [#1723](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1723) Error in console when typing in search field
    * Fixes a minor error that appeared in console when searching in lookup widgets.
  * [#1725](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1725) Tab not working in address modal window
    * Fixes a Bug in modal location editor window, now allowing to use Tab there again.
  * [#1730](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1730) Create purchase orders process - fields collapse
    * Improved Purchase Create action in sales order. Now not collapsing the tree after entering a Quantity value.
  * [#1734](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1734) Picking Terminal opens with all rows uncollapsed
    * Performance Improvement of Picking Terminal view, now opening collapsed and much faster.
  * [#1744](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1744) Table doesn't take the full available height
    * Fixes a Layout Issue in Grid View Presentation with Pagination widget.

# metasfresh 5.51 (2018-14)
**release for week 2018-14**

## Features
* metasfresh
  * [#3675](https://github.com/metasfresh/metasfresh/issues/3675) Introducing master documentno to give each contract chain a unique number
    * New Master Contract No created to allow the grouping of chanined subscription contracts.
  * [#3711](https://github.com/metasfresh/metasfresh/issues/3711) Contracts: Detect loops when extending a contract
    * Improvement of contracts prolongations, detecting a minor case where a loop could occur.
  * [#3725](https://github.com/metasfresh/metasfresh/issues/3725) Update to latest jasper & faster maven plugin
    * Performance improvement of the jasper build process, updated to latest jasper and maven plugin.
  * [#3776](https://github.com/metasfresh/metasfresh/issues/3776) Distribution Editor initial HU Assignment
    * Improved workflow in Distribution Editor Relocate action. Now the corresponding Handling Unit for the Distribution Orderline is initially selected.
  * [#3778](https://github.com/metasfresh/metasfresh/issues/3778) Automactically process picked CU's
    * Picking Improvement, now automatically processing picked CU's. In case of errors the user can reactivate again.
  * [#3784](https://github.com/metasfresh/metasfresh/issues/3784) Standalone BPartner Product Translation Window
    * New Window in WebUI that allows the maintenance of Business Partner Product Translations.

* metasfreh-webui-frontend
  * [#1586](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1586) Screen aliginment Improvements
    * Improves the Look & Feel, mostly vertical alignments - of all Fields and Field Content. Also Size of Lookup widget dropdowns.
  * [#1606](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1606) Searching in dropdown fields
    * New Feature allowing to search in List widgets via first character in List element.
  * [#1654](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1654) Provide support for time widgets
    * Adds support for Time-only widgets. Now not showing the date anymore.
  * [#1675](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1675) Tab Sequence
    * Improved Tab Sequence in generic Windows.

## Fixes
* metasfresh
  * [#3770](https://github.com/metasfresh/metasfresh/issues/3770) Solve issues around the print endpoint
    * Fixes different Bugs in print endpoint. Now its possible to use the printing service in WebUI.
  * [#3793](https://github.com/metasfresh/metasfresh/issues/3793) Cache: root documents are no longer invalidated
    * Cache improvment, now not invalidating root documents anymore.
  * [#3741](https://github.com/metasfresh/metasfresh/issues/3741) Credit Limit Detail Improvements
    * Detail improvements for the credit limit feature.
  * [#3748](https://github.com/metasfresh/metasfresh/issues/3748) Pharma: Regular import does not fail if prices aren't imported
    * Fixes a minor Bug in Pharma Product Import, now throwing an error in case the prices are not imported.
  * [#3761](https://github.com/metasfresh/metasfresh/issues/3761) Check Limit in BPartner changes from order to invoice
    * Credit Limit Improvement for check between Sales Order an Invoice.
  * [#3762](https://github.com/metasfresh/metasfresh/issues/3762) Check Limit in BPartner increases on purchase side
    * Bugfix in Credit Limit Check, now not increasing the credit limit when creating Purchase Orders.
  * [#3804](https://github.com/metasfresh/metasfresh/issues/3804) Error AnnotationConfigEmbeddedWebApplicationContext has not been refreshed yet
    * Internal Housekeeping Maintenance.

* metasfresh-webui-api
  * [#925](https://github.com/metasfresh/metasfresh-webui-api/issues/925) Picking terminal: sometimes picking slot vanishes
    * Fixes a Bug in WebUI Frontend. Eliminates cases in which the Picking Slot silently dissappeared from Screen.

* metasfresh-webui-frontend
  * [#1679](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1679) Layout bug with resolution 1920x1200
    * Fixes a Layout Bug in table header of Grid View, now showing the cells in initial S, M, L sizes again.
  * [#1700](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1700) attribute filter fields are shrinked
    * Fixes the Filter for Attributes e.g. in Window Businesspartner. Now it's able to use the filter again.

# metasfresh 5.50 (2018-13)
**release for week 2018-13**

## Features
* metasfresh
  * [#3585](https://github.com/metasfresh/metasfresh/issues/3585) WebUI window design: Business Partner Credit Limit
    * Improvement of Business Partner Credit Limit Field Names and Translations.
  * [#3687](https://github.com/metasfresh/metasfresh/issues/3687) Replace flags from tax category with a list
    * Adjustments on Tax Category that replaces checkboxes with a dropdown list for better maintainability.
  * [#3693](https://github.com/metasfresh/metasfresh/issues/3693) Lot-No lock & control
    * New Feature that allows the control and lock of Lot-No.
  * [#3703](https://github.com/metasfresh/metasfresh/issues/3703) Material Receipt Candidates Window, add media types for mobile/ tablet
    * Mobile Usage Improvement. Adds Mediatypes to Material Receipt Candidates window (Tablet prototype).
  * [#3716](https://github.com/metasfresh/metasfresh/issues/3716) Implement MSV3 server
    * New MSV3 Communication Service - Order and availaibilty check - for german Pharma Industry.
  * [#3721](https://github.com/metasfresh/metasfresh/issues/3721) Create Request on DD_Order to Quarantine warehouse
    * Now also creating a Request in case of Material Movements to Quarantine Warehouse.
  * [#3724](https://github.com/metasfresh/metasfresh/issues/3724) Allow to run print endpoint as standalone service
    * New Printing endpoint that allows the printing to be run as standalone service.
  * [#3738](https://github.com/metasfresh/metasfresh/issues/3738) Introduce and use AD_OrgInfo.M_WarehousePO_ID
    * Default Warehouse for an Organisation to be used when automatically creating Purchase Orders and as initial Warehouse selection.
  * [#3743](https://github.com/metasfresh/metasfresh/issues/3743) Translation of Distribution Editor Quickaction
    * Translation added for the Distribution Editor Quickactions.
  * [#3749](https://github.com/metasfresh/metasfresh/issues/3749) Add isPrintPrice flag in orderLine
    * New flag that allows to manually define if prices shall be printed in a Order document or not.
  * [#3758](https://github.com/metasfresh/metasfresh/issues/3758) Notify users if msv3-server was not reached
    * Improvement of the communication with an MSV3 Server in Sales Order, now letting the user know if a connection failed.

* metasfresh-webui-api
  * [#911](https://github.com/metasfresh/metasfresh-webui-api/issues/911) HU attributes shall consider M_HU_PI_Attribute.IsDisplayedUI flag
    * Now it's possible to track Attributes in Handling Units but to not display them in Handling Unit Editor.
  * [#913](https://github.com/metasfresh/metasfresh-webui-api/issues/913) Add switch for synchronous availiability check
    * New configuration swith that allows to switch between sync and async availability checks in MSV3 communication.
  * [#919](https://github.com/metasfresh/metasfresh-webui-api/issues/919) Allow to display only positive ATP values in product lookup
    * Improvement of the Availability check result in MSV3 Sales Orderline. Now only showing results with Available to promise > 0.

* metasfresh-webui-frontend
  * [#1680](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1680) Camera Barcode workflow improvements
    * Detailed improvements in the Barcode workflow for Tablet usage.
  * [#1681](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1681) Data Entry via barcode scan in Action Parms
    * New Functionality for Barcode Scanning in Action Parms.
  * [#1684](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1684) Combine dropdown list of <List> and <Lookup> component
    * Improvement of Lookup Widgets and List Components, combined functionality  for better maintainability.
  * [#1692](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1692) Detailed adjustments of User Interface for tablet media size
    * UI Improvement for Mobile/ Tablet Usage of storage relevant workflows.
  * [#1706](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1706) Dropdown bug in modal windows
    * Fixes the refactored Lookup & List widgets behavior.

## Fixes
* metasfresh
  * [#3698](https://github.com/metasfresh/metasfresh/issues/3698) NPE when clicking on picking-slot in swing picking terminal first time
    * Minor fix for a Null Pointer exception in Swing Client Picking Terminal.
  * [#3717](https://github.com/metasfresh/metasfresh/issues/3717) Swing - Bereitstellung POS hangs
    * Fixes the Window for Distribution order Handling in Java Swing Client.
  * [#3728](https://github.com/metasfresh/metasfresh/issues/3728) Cannot create material receipt if the ADR attribute is disabled in PI template
    * Fix for Material Receipt creation in case of disabled ADR Attribute.
  * [#3736](https://github.com/metasfresh/metasfresh/issues/3736) Jasper: Qty TU in purchase invoice is wrong again
    * Fixes the Quantity of transportation units in Purchase Invoice.
  * [#3739](https://github.com/metasfresh/metasfresh/issues/3739) Toplevel TUs are created as aggregate HUs
    * Solves issues in Handling Units that created Toplevel Handling Units as aggregated elements.
  * [#3746](https://github.com/metasfresh/metasfresh/issues/3746) ZoomTo - exception in console if IsGenericZoomOrigin='N'
    * Solves an issue that prevented Document References to be shown.
  * [#3755](https://github.com/metasfresh/metasfresh/issues/3755) Error in search of Businesspartner
    * Fixes the SQL of a virtual column in C_BPartner Table.

* metasfresh-webui-frontend
  * [#1605](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1605) Scrolling in dropdown fields
    * Fixes the behavior of dropdown fields when scrolling through the list.
  * [#1641](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1641) Combined Lookup Widget Layout Glitch
    * Fixes a Layout Glitch in combined Lookup Fields.
  * [#1649](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1649) Date range widget needs to support 2018-05-01 to 2019-04-30
    * Fixes the date timezone in date widgets.
  * [#1660](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1660) Single Date Field not patched in some cases
    * Fix for the patching of date fields when manipulating in mouse and keyboard combination.
  * [#1663](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1663) Pos1 does not jump to page 1 anymore
    * Fixes the Home Button in grid View. Now possible to jump to first page in Pagination again.
  * [#1676](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1676) List widgets with focus follow-up
    * Fixe for the List widget, now losing the focus indicator again when moving to other field.
  * [#1705](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1705) Barcode Scan leaved Webcam switched on
    * Now the Webcam is switched off as soon the Barcode reading process is finished.
  * [#1712](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1712) Dropdown list in grid view does not open with mouse click
    * Fixes the behavior of List and Lookup widgets in Subtab Grid View after double click.


# metasfresh 5.49 (2018-12)
**release for week 2018-12**

## Features
* metasfresh
  * [#3240](https://github.com/metasfresh/metasfresh/issues/3240) Drop AD_Field.IsCentrallyMaintained database column
    * Internal Housekeeping Issue, taking care of legacy column "isCentrallyMaintained".
  * [#3584](https://github.com/metasfresh/metasfresh/issues/3584) Implement sales order candidates REST API
    * New REST-API for order candidates. This is part of the new Pharma Availability Check and Ordering Service.
  * [#3658](https://github.com/metasfresh/metasfresh/issues/3658) Introduce specific subtypes for Physical Inventory and for Internal Use Inventory
    * Additional Document Subtypes for Physical Inventory and Internal usage.
  * [#3659](https://github.com/metasfresh/metasfresh/issues/3659) Refactor/adapt Inventory Disposal
    * Improvement of the Inventory disposal functionality. Adapting to new Inventory Control.
  * [#3669](https://github.com/metasfresh/metasfresh/issues/3669) Create all periods of a contract on creation
    * Improving the contract creation, now creating all periods at the moment of contract generation.
  * [#3688](https://github.com/metasfresh/metasfresh/issues/3688) Port Printing REST endpoint from SMX to metasfresh
    * Ports the REST Endpoint for Printing from ServiceMix to metasfresh.
  * [#3705](https://github.com/metasfresh/metasfresh/issues/3705) Inventory Window show Handling Unit Field in Inventorylines
    * Adds the Handling Unit into Inventopylines allowing to use Inventory with our Handling Usage Management.
  * [#3706](https://github.com/metasfresh/metasfresh/issues/3706) Terminating a Contract that was extended ahead of schedule leaves stumb
    * Improvement of the contract Termination action.
  * [#3718](https://github.com/metasfresh/metasfresh/issues/3718) Contracts: Transform IsAutoRenew and IsAutoExtension flags in a list

* metasfresh-api
  * [#894](https://github.com/metasfresh/metasfresh-webui-api/issues/894) New Composed Primary Keys
    * Allows now to use composed primary keys in WebUI.
  * [#895](https://github.com/metasfresh/metasfresh-webui-api/issues/895) Automatic printing HU Labels in WebUI
    * New Feature to automatically print TU Labels for Picking in WebUI.
  * [#901](https://github.com/metasfresh/metasfresh-webui-api/issues/901) Provide media size info for columns
    * Enhances the UI Element Configuration in Application Dictionary. It's now possible to define media size dependant behavior for the Web User Interface.
  * [#910](https://github.com/metasfresh/metasfresh-webui-api/issues/910) 2nd orderline for product missing in picking terminal
    * Now shows the 2nd Orderline in Picking Terminal again.

* metasfresh-webui-frontend
  * [#1609](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1609) Camera barcode reader for Tablet/ mobile device
    * New Barcode Reader that can be used via webcam on mobile devices.
  * [#1677](https://github.com/metasfresh/metasfresh-webui-frontend/pull/1677) Update momentjs in packages.json
    * Updateing Moments.js to the newses Version.
  * [#1699](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1699) Tab does not trigger saving number field
    * Fixes the patching in number fields. Now also patching when leaving the Fields via Tab Key.
  * [#1860](https://github.com/metasfresh/metasfresh/issues/1860) Make documentNo readonly in Payments (and other document types)
    * Improves the documetNo behavior, making all Fields with Document No read-only.

## Fixes
* metasfresh
  * [#3050](https://github.com/metasfresh/metasfresh/issues/3050) Null in SSCC label
    * Fix for the LotNo on SSCC Labels. If not set, the Lot No now shows an empty string instead of null.
  * [#3497](https://github.com/metasfresh/metasfresh/issues/3497) Days Due in Open Items report empty when parameter not set
    * Fixes the Parm description in Open Items report in WebUI, now showing "Unlimited" when the Dates Dues Parm is left empty.
  * [#3579](https://github.com/metasfresh/metasfresh/issues/3579) SSCC18 attribute check digit
    * Fixes the check digit of generated SSCC Numbers.
  * [#3666](https://github.com/metasfresh/metasfresh/issues/3666) Manufacturing Order wrong TU Quantity
    * Fixes the Qty of TU in Manufacturing Orders when automatically created after sales order complete (lot-for-lot).
  * [#3690](https://github.com/metasfresh/metasfresh/issues/3690) Restore swing MRP ProductInfo
    * Fixes the old MRP Product Info Window in Java Swing UI.
  * [#3694](https://github.com/metasfresh/metasfresh/issues/3694) docs_flatrate_term_all_procurements_conditions_report fails if M_Product_ID is left empty
    * Fixes the procurements conditions report. Now not failing anymore when the Product ID is left empty.
  * [#3695](https://github.com/metasfresh/metasfresh/issues/3695) NPE when completing DD_Order
    * Fixes a Null Pointer Exception that occurred sometimes when completung a Distribution Order.
  * [#3701](https://github.com/metasfresh/metasfresh/issues/3701) Jasper: ADR Auswertung report has duplicates
    * Removing Duplicate entries in the Swiss fresh produce ADR report.
  * [#3745](https://github.com/metasfresh/metasfresh/issues/3745) Compensation Group: Sequence of Lines is lost on Clone
    * Fixes the sequence of lines in Compensation groups when cloning a sales order document.

* metasfresh-webui-api
  * [#735](https://github.com/metasfresh/metasfresh-webui-api/issues/735) Hide Receive HUs (default) when there are no HUs
    * Hides the default action for Receive HU in cases where there are only CU's in receipt candidates.

* metasfresh-webui-frontend
  * [#1642](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1642) Lookup Widget drop-down list scroll behavior
    * Improves the behavior of drop-down list scroll behavior.
  * [#1669](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1669) Empty option missing in dropdown
    * Fixes the empty selected elements in list widgets after selecting entry.
  * [#1673](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1673) Improve User Interface for tablet media size
    * Layout adjustments for the usage of webui frontend on tablet media sizes.
  * [#1689](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1689) Scrollbar not shown in order window for subtab order lines
    * Fixes the missing horizontal Scrollbar.

# metasfresh 5.48 (2018-11)
**release for week 2018-11**

## Features
* metasfresh
  * [#2647](https://github.com/metasfresh/metasfresh/issues/2647) Inventory Functionality w/ Handling Unit Assignments
    * Improved Inventory Functionality for WebUI, now allowing to record Handling Unit quantities too.
  * [#3029](https://github.com/metasfresh/metasfresh/issues/3029) WebUI: New Window for Import Formats
    * New Indow in WebUI for Import Formats, now allowing to maintain data formats to import migration data.
  * [#3580](https://github.com/metasfresh/metasfresh/issues/3580) TU label in picking process in webui
    * New Action in Picking, allowing to print a Transport Unit Label.
  * [#3622](https://github.com/metasfresh/metasfresh/issues/3622) Make AD_EventLog available for admin
    * Improved Event Log Handling, now making the logs available for the admin role.
  * [#3634](https://github.com/metasfresh/metasfresh/issues/3634) Pick in manufacturing Order: Picking Slot Filter on selected BPartner from Shipment Schedule
    * New functionality in Manufacturing Workflow, allowing to directly pick produced products via manufacturing receipt workflow.
  * [#3637](https://github.com/metasfresh/metasfresh/issues/3637) Standalone Product Translation Window
    * New Standalone Product Translation window in WebUI.
  * [#3652](https://github.com/metasfresh/metasfresh/issues/3652) WebUI: New Inventory Window
    * New Window in WebUI that allows the maintenance of Inventory recordings and adjustments.
  * [#3591](https://github.com/metasfresh/metasfresh/issues/3591) Add translations for headers in shipment statistics
    * New WebUI window for shipment statistics.
  * [#3618](https://github.com/metasfresh/metasfresh/issues/3618) Add "technical note" field to AD_Column
    * Internal Housekeeping Improvement, adding a new Field to Application Dictionary in Column, that allows to record additional internal information.
  * [#3620](https://github.com/metasfresh/metasfresh/issues/3620) Spring model interceptors: support those who implement IModelInterceptor
    * Internal Housekeeping improvement, now discovering interceptors which implement the IModelInterceptor interface.
  * [#3621](https://github.com/metasfresh/metasfresh/issues/3621) Allow semicolon delimiter for Import Format
    * Enhancement of possible Import Delimiters in Import Format, now also allowing semicolon as delimiter.
  * [#3624](https://github.com/metasfresh/metasfresh/issues/3624) Pharma: When Operation Code is 2, deactivate the product
    * Improvement of the Import of Pharma Products, now dectivating Products with status code 2 (discontinued Products).
  * [#3674](https://github.com/metasfresh/metasfresh/issues/3674) Support Country in local address sequence
    * Now supporting the county variable in the local Address sequence.
  * [#3655](https://github.com/metasfresh/metasfresh/issues/3655) POJOWrapper support for model classes with zero ID
    * Internal Development improvement.
  * [#3667](https://github.com/metasfresh/metasfresh/issues/3667) Prospect is converted to customer when completing a quotation
    * Improvement of the prospect-customer transition, now setting to customer as soon first Partner Sales Order is completed.

* metasfresh-webui-api
  * [#773](https://github.com/metasfresh/metasfresh-webui-api/issues/773) Add name and menu entry for WebUI window Package
    * New Window in WebUI for Package maintenance.
  * [#882](https://github.com/metasfresh/metasfresh-webui-api/issues/882) WebUI: Pimp Data Import window
    * New Window for Date Import in WebUI. now allows to do the data import into metasfresh with drag&drop file attachment upload.

* metasfresh-webui-frontend
  * [#1640](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1640) Drag and Drop Attachments
    * Adds the functionality to upload multiple files at once.

* metasfresh-dist
  * [#35](https://github.com/metasfresh/metasfresh-dist/issues/35) Remove swing-client exe via launch4j
    * Internal Development improvement.

## Fixes
* metasfresh
  * [#3612](https://github.com/metasfresh/metasfresh/issues/3612) Sorting defect: Change of Flatrate Term in Sales Orderline after grouping
    * Fixes the Sorting in recreated Compensation group lines in sales order.
  * [#3639](https://github.com/metasfresh/metasfresh/issues/3639) Material dispo - problem with multiple cost collectors
    * Fixes an Issue in Material Disposition when receiving multiple Handling Units in manufacturing Order resulting in multiple cost collectors.

* metasfresh-api
  * [#850](https://github.com/metasfresh/metasfresh-webui-api/issues/850) Sorting by Virtual Column Follow-up
    * Fixes the sorting of virtual columns which are not numbers in grid view.
  * [#890](https://github.com/metasfresh/metasfresh-webui-api/issues/890) Exception when adding request from partner window for sales rep
    * Fixes a Bug in the Request creation action when started from partner window.

* metasfresh-webui-frontend
  * [#1544](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1544) List Widget does not scroll down with arrow-down
    * Improved scrolling behavior of list widgets.
  * [#1557](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1557) Double click on attributes in orderline
    * Improves the behavopr of the attributes dropdown widget when double clicking cell in subtab grid view. Now the elements are not all selected.
  * [#1615](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1615) Picking terminal window: switching rows is very very slow
    * Performance Improvement of Picking Terminal Window.
  * [#1637](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1637) Collapsible lines in Create Purchase Order modal
    * Fixes the behavior of collapsible lines in modal overlay of create purchase orders.
  * [#1646](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1646) List dropdown improvements
    * Improved behavior of lookup and list widget drop-down. Now keeping the field content selected when reopening the drop-down after hover and leave.
  * [#1650](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1650) Edit mode in grid view when focus lost
    * Improvement of the display status of grid fields in edit mode. Now the edit modus and display is left as soon the field is left.
  * [#1651](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1651) Multi Line Text Field ist not patched when text is removed
    * Fixes the patching of empty Text Fields.
  * [#1653](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1653) Line in modal overlay for creating purchase order from SO disappears
    * Fixes an Issue in Create Purchase Orders from Sales Order Lines. Now it's possible to enter the purchase Quantity again.
  * [#1658](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1658) Improve WebUI performance
    * General Performance Improvement for Grid Views in WebUI.
  * [#1662](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1662) Attributes in OrderLine grid view are not saved
    * Fixes the recording of attributes in document lines. Now they are saved again.

# metasfresh 5.47 (2018-10)
**release for week 2018-10**

## Features
* metasfresh
  * [#3540](https://github.com/metasfresh/metasfresh/issues/3540) WebUI: Show GuaranteeDaysMin on Product and Product Category windows
    * Improved Product and Product Category windows, added new field for Min. Guarantee Days ad part of the best before management.
  * [#3541](https://github.com/metasfresh/metasfresh/issues/3541) Div material dispo issues
    * Implements various detailed features in the material disposition feature.
  * [#3549](https://github.com/metasfresh/metasfresh/issues/3549) Refactor config for Distribution Order/ Movement after Material Receipt
    * Improvement of the new Distribution Order generation after material receipt to allow a better understanding of configuration switches.
  * [#3556](https://github.com/metasfresh/metasfresh/issues/3556) Webui: Pimp Compensation Group Schema window
    * Enhanced Window Compensation group Schema, added fields for the new automatic Discount Functionality.
  * [#3561](https://github.com/metasfresh/metasfresh/issues/3561) Add relation between Invoice and Shipment Constraint
    * New relation added for the navigation between invoices and shipments.
  * [#3562](https://github.com/metasfresh/metasfresh/issues/3562) Primary Layout in Product Planning Subtabs
    * Layout adjustment for the Subtabs in Product planning window, now added primary background to all of them.
  * [#3565](https://github.com/metasfresh/metasfresh/issues/3565) Initial Promised Date calculation and default Preparation Date
    * New Feature that allows to calculate an initial promised date in sales order based on date ordered.
  * [#3570](https://github.com/metasfresh/metasfresh/issues/3570) CustomerLabelName in M_Product and Translation
    * New translateable field in the product masterdata that allws to record the default Customer Label Name for a product.
  * [#3575](https://github.com/metasfresh/metasfresh/issues/3575) Make shipment HU aggregation configurable
    * New feature that allows to configure the aggregation of shipment lines for shipped Handling Units.
  * [#3576](https://github.com/metasfresh/metasfresh/issues/3576) TU label in picking
    * New Label for Transportation Units that can be created in the picking workflow.
  * [#3578](https://github.com/metasfresh/metasfresh/issues/3578) Introduce AD_Column.IsForceIncludeInGeneratedModel to force including a column to generated java models
    * Internal Housekeeping issue that allows to force include columns in model generation no matter what entity type the corresponding table has.
  * [#3582](https://github.com/metasfresh/metasfresh/issues/3582) Avoid mass-creation of "MissingShipmentSchedulesWorkpackages"
    * Performance Improvements to the Subscription evaluation process, now avioiding the creation of mass work packages when not needed.
  * [#3588](https://github.com/metasfresh/metasfresh/issues/3588) Drop support for org.adempiere.server.embedded
    * Internal Housekeeping improvement.
  * [#3587](https://github.com/metasfresh/metasfresh/issues/3587) Implement user token authentication for future REST APIs
    * Implementation for the user token authentication to our REST APIs.
  * [#3590](https://github.com/metasfresh/metasfresh/issues/3590) Make shipment line attribute set instance (ASI) configurable
    * New Feature that allows to configure the creation of shipment line Attributre set instances instead of just creating a copy from sales orderline.
  * [#3592](https://github.com/metasfresh/metasfresh/issues/3592) Add invoice related virtual columns in Shipment Restrictions
    * New searchable Fields in Shipment Restrictions for Invoice ID and isPaid.
  * [#3599](https://github.com/metasfresh/metasfresh/issues/3599) Pharma: Use IFA category when importing IFA products
    * Now using the IFA Category as Product Category after Import of Pharma Products.
  * [#3604](https://github.com/metasfresh/metasfresh/issues/3604) Provide AD_Window_ID to running process
    * Improvement of the Process Info, now adding the Window ID to it and storing it in the Process Instance record. This allows to retrieve more infomration about from where a Process was triggered.
  * [#3605](https://github.com/metasfresh/metasfresh/pull/3605) Add mvnw so that users don't need to install mvn to build from cmdline
    * Internal Housekeeping solution for maven build via commandline.
  * [#3609](https://github.com/metasfresh/metasfresh/issues/3609) Default Product Window take out Pharma specific fields
    * Adjustment of the default product window, removing all pharma vertical fields. These are included in the Pharma product window.

* metasfresh-webui-api
  * [#878](https://github.com/metasfresh/metasfresh-webui-api/issues/878) Distribution Editor Move HU dropdown list HU
    * Improvement of the Move Handling Unit Action in distribution editor, now pre-filtering the entries and matching base data.
  * [#879](https://github.com/metasfresh/metasfresh-webui-api/issues/879) Import File Loader substitute in WebUI
    * New feature in Webui as substitute for the file-loader form in swing client. This enables the import of date via webui.
  * [#880](https://github.com/metasfresh/metasfresh-webui-api/issues/880) Collapse Purchase Order dispo in Sales Order modal
    * Improved visibility in Create Purchase Order from Sales Orderlines, now collapsing the top level entries initially.
  * [#883](https://github.com/metasfresh/metasfresh-webui-api/issues/883) HU Labels in WebUI
    * Refined Handling Unit Labels actio now available in WebUI Handling Unit Editor.
  * [#886](https://github.com/metasfresh/metasfresh-webui-api/issues/886) Field Readonly = 'Y' but still updateable in WebUI
    * Refined Implementation of the Field Readonly Logic in Application Dictionary.

* metasfresh-webui-frontend
  * [#1620](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1620) List widgets with focus shall have dark grey color underline
    * Improved focus indicator line for list widgets.
  * [#1621](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1621) Dropdown List Widget - first entry at top shall be selected entry
    * Improves the behavior of selected elements in List drop-downs. Now showing them as first entry in list.
  * [#1622](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1622) List widget with only 1 entry shall still show the drop-down
    * Now the List widget also shows a drop-down list with only 1 entry.
  * [#1635](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1635) Check code formatting on CI
    * Adding code formatting rules to continuous integration platform.
  * [#1644](https://github.com/metasfresh/metasfresh-webui-frontend/pull/1644) Add cypress e2e test setup
    * Adding cypress setup for end-2-end tests of the webui frontend project.


## Fixes
* metasfresh
  * [#3422](https://github.com/metasfresh/metasfresh/issues/3422) Material Cockpit Document Details Doctype, DocNo wrong/ missing
    * Fixes the document detailes modal overlay in material cockpit. Now showing the document details with document no and document type.
  * [#3569](https://github.com/metasfresh/metasfresh/issues/3569) Purchase order from purchase candidate not working 
    * Fixes a bug that prevented the automatic creation of purchase orders from purchase candidates.
  * [#3571](https://github.com/metasfresh/metasfresh/issues/3571) AD_Element_trl problem with autocomplete fields
    * Fixes an issue that occurred when adding translation elements via autocomplete widgets.
  * [#3572](https://github.com/metasfresh/metasfresh/issues/3572) Internal usage (Materialentnahme partial) broken
    * Fix for the internal usage action when removing partial customer unit quantities, mostly weight unit of measure.
  * [#3595](https://github.com/metasfresh/metasfresh/issues/3595) Tax Error on w101 Sales Order Batch entry
    * Improved error message for Tax errors, now elaborating more whats the reason for the errors.
  * [#3644](https://github.com/metasfresh/metasfresh/issues/3644) "No Selection" error when generating shipments
    * Improvement of action/ Quickaction availability in Shipment Schedule. Now only showing line dependent actions if a line is selected. 

* metasfresh-webui-frontend
  * [#1550](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1550) Dropdown List Widget does not show 1st line as selected with keyboard scroll
    * Now the field content is shown as selected first element in the dropdown.
  * [#1623](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1623) Attributes not shown in Material Receipt Candidates
    * Fixes a Bug in the Handling Unit Editor in Material Receipts, not showing the Attributes View when Receiving CU.
  * [#1625](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1625) Show Attribute Editor for selected CU Level HU
    * Fix for the Handling Unit Editor when selectin the first entry of an HU. Now initially showing the Attributes view again.
  * [#1628](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1628) Clicking in field w/ 1 value in dropdown sets the value directly
    * Fixes the List widget with only 1 entry. Now opening the list widget drop-down instead of directly setting the single entry.
  * [#1630](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1630) Setting attributes in orderline not working
    * Fixes the Listr widget for attributes in document lines.
  * [#1638](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1638) Cannot use the dropdown in login
    * Fixes the dropdown widget in login window.
  * [#1645](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1645) Mandatory List Widget
    * Fixes the visibility for empty mandatory list widget fields.

# metasfresh 5.46 (2018-09)
**release for week 2018-09**

## Features
* metasfresh
  * [#3430](https://github.com/metasfresh/metasfresh/issues/3430) Best before Date evaluating process/ action
    * New action that analyzes the Handling Units on stock and marks them as "Best before" cases if the best-before-date has reached a time offset.
  * [#3503](https://github.com/metasfresh/metasfresh/issues/3503) Use correct picking quantities in shipment
    * Improvement of shipment document lines generation. Adjusting the base data to fill the picking quantities in shipment.
  * [#3513](https://github.com/metasfresh/metasfresh/issues/3513) Webui: Pimp DATEV windows
    * New Windows for accounting export and export formats in webui.
  * [#3515](https://github.com/metasfresh/metasfresh/issues/3515) Webui: Pimp Compensation Group Schema window
    * New Window for Compensation group maintenance.
  * [#3516](https://github.com/metasfresh/metasfresh/issues/3516) Price/ Discount Change restrictions Order/ Invoice Pharma
    * New feature that allows to restrict user changes on discounts and prices during sales order recording, depending on the configuration in product prices.
  * [#3532](https://github.com/metasfresh/metasfresh/issues/3532) New Window for Shipment Statistics
    * New Window that shows shipment statistics and allows to filter and export as excel file.
  * [#3534](https://github.com/metasfresh/metasfresh/issues/3534) Webui Window Design: Create window for Picking Config
    * New Window for Picking group Configuration.
  * [#3537](https://github.com/metasfresh/metasfresh/issues/3537) Remove legacy M_Production code
    * Internal housekeeping, removing some old/ unused M_Production code.
  * [#3555](https://github.com/metasfresh/metasfresh/issues/3555) Automatic Group Discount Calculation
    * New action in Sales order that allows to group lines and automatic select the appropriate discount depending on quantities and amount breaks.
  * [#3557](https://github.com/metasfresh/metasfresh/issues/3557) Respect Picking Group Selection in Picking HU Editor
    * Improved Handling Unit Filterin in Picking, now also respecting the newly introduces Picking Groups.

* metasfresh-webui-api
  * [#820](https://github.com/metasfresh/metasfresh-webui-api/issues/820) Picking Terminal: Detailed Picking Issues
    * Improvents of some workflow and filtering details (overdelivery allowed, initial quantities calculated and set in picking action, initially retrieving and setting the packing instructions) in the new picking Terminal in WebUI.
  * [#857](https://github.com/metasfresh/metasfresh-webui-api/issues/857) Material Cockpit additional Filter criteria
    * New Filter criteria added in the Material Cockpit.
  * [#876](https://github.com/metasfresh/metasfresh-webui-api/issues/876) Preset Product and Qty in Process/ Action Pick CU
    * Improved workflow in Pick Customer Unit Action. Now presetting the product and the remaining quantity to pick.
  * [#870](https://github.com/metasfresh/metasfresh-webui-api/issues/870) Extend Attribute / Label Feature to support tab link columns / Foreign Key
    * Improvement of the Label Feature, now allowing to link to the subtabs parent link column when set.
  * [#877](https://github.com/metasfresh/metasfresh-webui-api/issues/877) Picking tray Clearing action: Take out and add to new/ existing HU
    * New action that allows to take aout multiple Customer Units at once and add them to a new or existing Package Handling Unit.

* metasfresh-webui-frontend
  * [#1554](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1554) Action Parm modal Overlay focus missing n 1st Field
    * Improves the behavior of focused List widgets. Now the drop-down list is only opened if the user presses arrow-down.

## Fixes
* metasfresh
  * [#3452](https://github.com/metasfresh/metasfresh/issues/3452) Material Receipt candidates serial No - TU-CU case
    * Minor fix for the Handling Unit Serial No. distribution in material receipt. Now also working when selecting Transport units and Customer Units together.
  * [#3520](https://github.com/metasfresh/metasfresh/issues/3520) Workpackage with error for Update Invalid Shipment Schedules
    * Internal Housekeeping, solving an issue with a corercase in async workpackage processing.

* metasfresh-webui-frontend
  * [#1394](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1394) Quickactions not loaded after using barcode/ std. filter in HU editor in Manufacturing Order
    * Fixes a Bug that let the Quickactions Buttons disappear after setting filter criteria.
  * [#1567](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1567) Create purchase orders: Date promised format
    * Fixes the date/ time format in create puchase orders modal overlay in sales order.
  * [#1585](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1585) Date recording with keys leads to error
    * Fixes a Bug that occurred when trying to record a date via keyboard instead of calendar widget.
  * [#1604](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1604) Date Range Picker shows wrong day of the week
    * Fixes the shown day of week in date range picker.

* metasfresh-webui-api
  * [#856](https://github.com/metasfresh/metasfresh-webui-api/issues/856) t_query_selection grows huge when importing products or partners massively
    * Improved processing of the Query Selection when doing a Businesspartner or Products Import with large datasets.
  * [#859](https://github.com/metasfresh/metasfresh-webui-api/issues/859) Navigation Menu shown duplicated for Windows not in Menu
    * Fixes the Breadcrumb navigation menu for windows that are not included in WebUI menu. Now not showing a duplicated drop-down list anymore.
  * [#860](https://github.com/metasfresh/metasfresh-webui-api/issues/860) Shipment disposition does not update when you complete the order
    * Fix for the shipment schedule recompute after sales order complete. Now updated correctly again so the picking terminal is now shown correctly in document reference list again.
  * [#863](https://github.com/metasfresh/metasfresh-webui-api/issues/863) Fix available stock (ATP) display in sales order
    * Fixes the available to promise information in sales orderline batch entry.
  * [#869](https://github.com/metasfresh/metasfresh-webui-api/issues/869) Sometimes the error message is in German even if I am logged in with English
    * Minor fix for the translation of error messages. In some cases the error messages were shown in the base language instead of the language the user was logged in.
  * [#871](https://github.com/metasfresh/metasfresh-webui-api/issues/871) Error when selecting tabs in bpartner window
    * Fixes a cornercase that occurred when seleting included tabs in the businesspartner window in WebUI for records that were recorded via swingUI.
  * [#872](https://github.com/metasfresh/metasfresh-webui-api/issues/872) Don't show passwords in grid view
    * Fixes the password fields in Webui Grid View, now showing them obfuscated too, like in main view.

# metasfresh 5.45 (2018-08)
**release for week 2018-08**

## Features
* metasfresh
  * [#2777](https://github.com/metasfresh/metasfresh/issues/2777) Vendor Invoice Layout and Translations in WebUI Improvements
    * Adds Translations and Layout Impovement to Purchase Invoice window.
  * [#3246](https://github.com/metasfresh/metasfresh/issues/3246) Barcode Search in Handling Unit Editor takes too long
    * Improved Performance in handling Unit Editor when searching via Barcode Filter and Default Filter Handling Unit Value.
  * [#3409](https://github.com/metasfresh/metasfresh/issues/3409) Distribution Order/ Movement after Material Receipt
    * Adds an automatism Functionality to Product Plannung. Allows to automatically create Distribution Orders to bring received goods to their locators after material receipt.
  * [#3414](https://github.com/metasfresh/metasfresh/issues/3414) Credit Limit check in Sales Order
    * New Functionality in Sales Order, now checking the customers credit limit when completing the Order.
  * [#3437](https://github.com/metasfresh/metasfresh/issues/3437) MSV3 handle deviating response from remote MSV3 server
    * Improved communication between MSV3 Server and response presentation to the user.
  * [#3451](https://github.com/metasfresh/metasfresh/issues/3451) Extract esb code into dedicated repo
    * Internal housekeeping improvement, moving the code for enterprise service bus to dedicated repository.
  * [#3457](https://github.com/metasfresh/metasfresh/issues/3457) Improve performance around update_trl_tables_on_ad_element_trl_update
    * Performance Improvement of the Translation update mechanisms.
  * [#3481](https://github.com/metasfresh/metasfresh/issues/3481) Force refreshing virtual column CreditLimitIndicator from C_BPartner
    * Now allowing a just in time refresh of the credit limit indicator in Business Partner Window.
  * [#3483](https://github.com/metasfresh/metasfresh/issues/3483) Default Value for process create order from quotation
    * Adds default parms to the create order from quotation process/ action.
  * [#3490](https://github.com/metasfresh/metasfresh/issues/3490) Paperless Credit Limit approval
    * Improved workflow for the credit limit approval. Now the responsible user receives a notification as soon a credit limit shall be approved.
  * [#3502](https://github.com/metasfresh/metasfresh/issues/3502) Default Filter Improvements
    * Adds various Filter criteria to default window filter lists.
  * [#3505](https://github.com/metasfresh/metasfresh/issues/3505) Improvement of Procurement Candidates
    * Usability Improvement of the procurement Planning window. Rearranged fields for better visibility.
  * [#3508](https://github.com/metasfresh/metasfresh/issues/3508) Implement DATEV export window
    * New window and Fucntionality in WebUI that allows to export the Accountings in metasfresh to Datev.

* metasfresh-webui-api
  * [#851](https://github.com/metasfresh/metasfresh-webui-api/issues/851) Virtual field from header doc shall be refreshed when one of the included row is changed
    * Just-in-time update of the windows content for Virtual columns.
  * [#853](https://github.com/metasfresh/metasfresh-webui-api/issues/853) Automatic group creation in sales order lines
    * New automatic grouping functionality in sales orderlines.
  * [#854](https://github.com/metasfresh/metasfresh-webui-api/issues/854) If the window is missing from menu render it's name in breadcrumb
    * Window Breadcrumb improvement, now showing the windowname of windows that were reached via zoom and are not in menu yet.

* metasfresh-webui-frontend
  * [#1596](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1596) Add Enzyme to test setup
    * Extending our Test Framework with Enzyme.

## Fixes
* metasfresh
  * [#3216](https://github.com/metasfresh/metasfresh/issues/3216) Invoice candidate: The isRecompute flag is not reseted on N ever
    * Fix for invoice Candidates, now not recomputing anymore when candidates are processed.
  * [#3357](https://github.com/metasfresh/metasfresh/issues/3357) SQL Exception in Window Entity Type
    * Fixes a SQL Exception that occurred in Entity Type window.
  * [#3465](https://github.com/metasfresh/metasfresh/issues/3465) Window Role Tab User Access shows non systemusers
    * Fixes the Subtab for Tab User Access in Role window. Now only showing available Systemusers.
  * [#3486](https://github.com/metasfresh/metasfresh/issues/3486) Material Disposition automatic entries missing for DD/ PP Orders
    * Fixes the creation of Distribution and Manufacturing Orders in material Disposition.
  * [#3499](https://github.com/metasfresh/metasfresh/issues/3499) Cannot create manual invoice
    * Fixes the functionality to create manual Invoices.
  * [#3521](https://github.com/metasfresh/metasfresh/issues/3521) Exception with CreditStatus in some data constellations
    * Minor Bugfixes for the new credit status functionality.

* metasfresh-webui-api
  * [#846](https://github.com/metasfresh/metasfresh-webui-api/issues/846) Cache issue in shipment schedules subtab
    * Fixes a cache issue in a shipment shedules included subtab.
  * [#847](https://github.com/metasfresh/metasfresh-webui-api/issues/847) Error in picking terminal
    * Fixes a Bug that occurred in Picking terminal when picking a large amount of Handling Units.
  * [#848](https://github.com/metasfresh/metasfresh-webui-api/issues/848) Sorting by Virtual Column manually in webui throws error
    * Fixes the possibility to order by for virtual column in grid view.

* metasfresh-webui-frontend
  * [#1592](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1592) Added subrow is still/again not shown in the frontend
    * Fixes the feature for included subrows and asynchronous reponse.


# metasfresh 5.44 (2018-07)
**release for week 2018-07**

## Features
* metasfresh
  * [#3405](https://github.com/metasfresh/metasfresh/issues/3405) Schema for Product Planning Data
    * New Feature that allows to define default Product Planning Data. These Schemas are used to ensure the automatic creation of proper distribution orders for newly imported products.
  * [#3406](https://github.com/metasfresh/metasfresh/issues/3406) Set Selector in M_Product after Product Data Import
    * New Selector Feature for Product Import allowing to join new Product Data to Product Planning Schema.
  * [#3407](https://github.com/metasfresh/metasfresh/issues/3407) New Businesspartner Window for Pharma vertical
    * New Business Partner Window in WebUI for Pharma Verticals.
  * [#3408](https://github.com/metasfresh/metasfresh/issues/3408) New Product Window for Pharma vertical
    * New Product Window in WebUI for Pharma Verticals.
  * [#3413](https://github.com/metasfresh/metasfresh/issues/3413) Credit Limit data structure as subtab in Businesspartner
    * New Credit Limit functionality. Now allowing to define Credit Limit per Customer on different levels.
  * [#3458](https://github.com/metasfresh/metasfresh/issues/3458) Remove M_Storage-based legacy check from MProduct
    * Internal housekeeping improvement, getting rid of old storage based checks.
  * [#3467](https://github.com/metasfresh/metasfresh/issues/3467) Preparation Date Filer as Date Range
    * Adjustment for the Preparation Date Filter in Manufacturing Order. Now is a Date Range filter instead of date.
  * [#3468](https://github.com/metasfresh/metasfresh/issues/3468) Add Translation for "All Dates available"
    * Adds the translation for en_EN, de_DE of the "Show all dates" hint in Date Range filter.
  * [#3471](https://github.com/metasfresh/metasfresh/issues/3471) Disable Sales Opportunities Window until its permission is configurable
    * Hiding the Sales Opportunity Window from default WebUI Menu, as long as in beta.
  * [#3487](https://github.com/metasfresh/metasfresh/issues/3487) Extend Identifier Transportation Order
    * Improving the Transportation Order identifier, now additionally showing Date and Tour.
  * [#3495](https://github.com/metasfresh/metasfresh/issues/3495) Improvements to Product Price Window
    * Improving Product Price Window in WebUI, adding Active indicator and removing Price Matching Order from grid View.

* metasfresh-webui-api
  * [#818](https://github.com/metasfresh/metasfresh-webui-api/issues/818) Values.valueToJsonObject() shall return JSONNullValue instead of null
    * Internal improvement of the Handling of null values in JSON Objects.

* metasfresh-webui-frontend
  * [#1501](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1501) Automated Javascript and React Testing with Jest
    * Kickoff of the autmated Testing Framework for metasfresh setup on Jest and Enzyme.
  * [#1590](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1590) Included tabs sorting
    * Improvement of the sorting functionality in main and included subtab Grid Views.
  * [#1593](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1593) Copy/ Paste for selected Field in Subtab GridView not giving correct result
    * New Feature that allows to mark a Field in Grid View and copy the field content to clipboard.
  * [#1598](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1598) Changes in location not always saved
    * Fixes the handling of the location recording.

## Fixes
* metasfresh
  * [#3445](https://github.com/metasfresh/metasfresh/issues/3445) Qty TU not correct in purchase invoice jasper
    * Fixes the Purchase Invoice document. Now the correct quantity of Handling units is shown again.
  * [#3477](https://github.com/metasfresh/metasfresh/issues/3477) Cannot save manufacturing order
    * Fixes an error in manufacturing order window, now allowing to save the order again.

* metasfresh-webui-api
  * [#806](https://github.com/metasfresh/metasfresh-webui-api/issues/806) Add to Transportation Order, Ship and Invoice action in Picking Clearing Tray not respecting the invoice schedule
    * Fixes the Action for automatic creation of invoices after picking & packing. Now the action is respecting special invoice schedules for the given customer.
  * [#807](https://github.com/metasfresh/metasfresh-webui-api/issues/807) Quantity to invoice override callout
    * Fixes a Bug when updating the Quantity to Invoice override. Now the effective quantity is updated again.
  * [#829](https://github.com/metasfresh/metasfresh-webui-api/issues/829) Planning status in manufacturing order not updated
    * Fixes an issue in Manufacturing Order, leaving the Planning Status unchanged after processing the order.

* metasfresh-webui-frontend
  * [#1546](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1546) Date Range Filter as Range Filter has initial daterange
    * Leaves the Daterange filter now initially empty to that it does not interrupt other filtering.
  * [#1553](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1553) Drop down lists remain displayed when using tab several times (again)
    * Fixes a Bug with dropdown lists staying open after tabbing away.
  * [#1558](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1558) Dropdown fields not hidden when creating a new Business Partner
    * Fixes the reamining dropdown in Purchase Order when calling the "New Businesspartner" action in context menu.
  * [#1559](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1559) Errors in the console when opening HU Editor
    * Fixes errors in console that popped up when opening the Handling Unit Editor.
  * [#1588](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1588) Zoom Into is not working
    * Fixes the Zoom-To functionality that allows the user to click on field labels and jump to detail data when available.

# metasfresh 5.43 (2018-06)
**release for week 2018-06**

## Features
* metasfresh
  * [#3410](https://github.com/metasfresh/metasfresh/issues/3410) Enlarge AD_Table.TableName
    * Resizing the Fields for Tablename in Applicaiton Dictionary, now allowing 80 chars.
  * [#3411](https://github.com/metasfresh/metasfresh/issues/3411) Implement MSV3 purchase order
    * New Feature in Pharma Vertical, allowing to create MSV3 Purchase Orders.
  * [#3417](https://github.com/metasfresh/metasfresh/issues/3417) Support new VAT rate of 7.7% in Switzerland from 01.01.2018
    * New Tax Masterdate for VAT in Switzerland valid from 01-01-2018.
  * [#3419](https://github.com/metasfresh/metasfresh/issues/3419) Throw meaningful exception if MOrderLine.beforeSave has problems
    * Improving error messages in Orderline, now returning meaningful information to the user.
  * [#3428](https://github.com/metasfresh/metasfresh/issues/3428) Switch off Daterange in Preparation date Filer temporarily
    * Changes the Filter of Preparation Date to simple Date instead of Daterange.
  * [#3438](https://github.com/metasfresh/metasfresh/issues/3438) Qty LU wrong in purchase invoice candidates / invoice
  * [#3439](https://github.com/metasfresh/metasfresh/issues/3439) Improvement of GO Delivery Order Window
    * Improved the visibility of important information in the GO! Delivery Window in WebUI.
  * [#3440](https://github.com/metasfresh/metasfresh/issues/3440) Improvement of Shipper Window in WebUI
    * Extends the Shipper Window in WebUI, now also allowing the recording of the GO! Shipper Configuration.
  * [#3454](https://github.com/metasfresh/metasfresh/issues/3454) Resolve log warning "Skip setting parameter value for X_AD_PInstance_Para[0]"
  * [#3455](https://github.com/metasfresh/metasfresh/issues/3455) Migitate "PO not handled: Document{tableName=M_InOut.." and similar warnings flooding the log

* metasfresh-webui-api
  * [#812](https://github.com/metasfresh/metasfresh-webui-api/issues/812) Picking Tray Clearing: Action take out and add to LU/ TU
    * New Action for Picking Tray Handling Unit removals and automatic adding to an exiting Logistics Unit.
  * [#815](https://github.com/metasfresh/metasfresh-webui-api/issues/815) Transform TU to exiting LU takes too long for Handling Unit Dropdown List
    * Performance Improvement of Transformation List Dropdown in HU Editor.
  * [#817](https://github.com/metasfresh/metasfresh-webui-api/issues/817) Include stacktrace when providing the error to frontend
    * Now providing the stacktrace from Backend to Frontend. Can be switched on in Frontend config for testing purpose.

* metasfresh-webui-frontend

## Fixes
* metasfresh
  * [#3022](https://github.com/metasfresh/metasfresh/issues/3022) Contracts: ContractDocumentNo is 0 all the time
    * Fixes the automatic Document No generation in Contracts, now not leaving Document No 0 there anymore.
  * [#3394](https://github.com/metasfresh/metasfresh/issues/3394) Sales inout Jasper: HU name taken from line
    * Fix for the Packing Instruction shown in Sales Inout Document when using manual Packing Material.
  * [#3402](https://github.com/metasfresh/metasfresh/issues/3402) Can't credit memo a partially paid invoice
    * Improvement of the status Handling after reopening Manufacturing Orders.
  * [#3449](https://github.com/metasfresh/metasfresh/issues/3449) ImportHelper doesn't switch ctx

* metasfresh-webui-api
  * [#617](https://github.com/metasfresh/metasfresh-webui-api/issues/617) Cache is not invalidated on country change
    * Fixes a Bug in Cache Invalidation for Country changes and Pricing.
  * [#801](https://github.com/metasfresh/metasfresh-webui-api/issues/801) Transforming aggregated CU with "CU to existing TU" not working correctly
    * Fixes an error in the "CU to existing TU" action.
  * [#802](https://github.com/metasfresh/metasfresh-webui-api/issues/802) Transforming aggregated CU with "CU to new TU" not working correctly
    * Fixes an error "CU to existing TU" action, sometime leaving wrong calculates quantities behind.
  * [#810](https://github.com/metasfresh/metasfresh-webui-api/issues/810) Update QtyPicked after picking
    * Fixes a Refresh Bug, leaving the Picked Quantities not updates after picking the Product.
  * [#811](https://github.com/metasfresh/metasfresh-webui-api/issues/811) Java Nullpointer Exception in special case with multiple attribute and multi column layout
    * Fixes a NPE in multi (>2) Column Layout Windows.

* metasfresh-webui-frontend
  * [#1528](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1528) Added subrow is not shown in the frontend
    * Improved response from MSV3 request so that purchase candidate row is shown and user can directly start editing.
  * [#1538](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1538) Date Fields not patched
    * Fixes an error with Date Fields, now patching them after changes again.
  * [#1543](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1543) Sales Order window Purchase Order modal overlay broken again
    * Fixes the Purchase Order modal overlay functionality in Sales Order.
  * [#1564](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1564) Some fields are not patched after you change them twice
    * Fixes the multiple adjustment behavior of Text and numeric fields. now content is patched after each change.
  * [#1566](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1566) Subtab Data not shown when clicked first time
    * Fixes a Refresh Bug in Subtab data. Now showing the actual data already when opening the subtab first time.
  * [#1570](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1570) Views: fails when applying a filter without parameters
    * Fixes the Filter. Now does not fail when applied without filter criteria.

# metasfresh 5.42 (2018-05)
**release for week 2018-05**

## Features
* metasfresh
  * [#3299](https://github.com/metasfresh/metasfresh/issues/3299) Automatic Picking
    * New Feature that allows to define Products in Planning Data, that shall be automatically picked after action receipt in manufacturing.
  * [#3302](https://github.com/metasfresh/metasfresh/issues/3302) Payment Discount on Orderline, Invoice Candidate
    * Adding a Payment Discount overwrite to Orderlines and Invoice Candidates. With this feature one can add Payment Discounts as additional Discount Schema entry.
  * [#3310](https://github.com/metasfresh/metasfresh/issues/3310) Webui Window Design: Improve window System Issue Report
    * New Window System Issue Report in WebUI, allowing teh System Administrator to check System Issues.
  * [#3313](https://github.com/metasfresh/metasfresh/issues/3313) Webui Window Design: Improve window Field Group
    * New Window in WebUI for Field Group maintenance. This window can be used by System Admins.
  * [#3317](https://github.com/metasfresh/metasfresh/issues/3317) Webui Window Design: Improve window Report & Process
    * New Window in WebUI for Process & Reports maintenance.
  * [#3318](https://github.com/metasfresh/metasfresh/issues/3318) Webui Window Design: Improve window Reference
    * New Window in WebUI for Reference maintenance.
  * [#3319](https://github.com/metasfresh/metasfresh/issues/3319) Webui Window Design: Improve window Message
    * Improvement of the WebUI message window.
  * [#3322](https://github.com/metasfresh/metasfresh/issues/3322) Webui Window Design: Improve window Validation Rule
    * New Window for the maintenance of Validation Rules in metasfresh. This window can be used by System Admins.
  * [#3329](https://github.com/metasfresh/metasfresh/issues/3329) Webui Window Design: Translate all in window Event store
    * Improved Window, Tab and Fields translations in the Event Store Window..
  * [#3330](https://github.com/metasfresh/metasfresh/issues/3330) Webui Window Design: Improve window Entity Type
    * New Window for the maintenance of Entity Types. This window can be used by System Admins.
  * [#3338](https://github.com/metasfresh/metasfresh/issues/3338) Harmonize description field length between doctype and c_order / c_invoice
    * Improvement of description fields in doctype. Now the fields in Order and Invoice doctype have the same field length.
  * [#3346](https://github.com/metasfresh/metasfresh/issues/3346) Remove rebel-remote.xml files
    * Internal Housekeeping improvement. Removing remote rebel files.
  * [#3347](https://github.com/metasfresh/metasfresh/issues/3347) Drop M_Product_Costing
    * Dropping the legacy Costing Functionality, making place for the new Costing Engine to come.
  * [#3349](https://github.com/metasfresh/metasfresh/issues/3349) Add BPartner to User Window
    * New Field in Window User, allowing to see and maintain the Business Partner.
  * [#3353](https://github.com/metasfresh/metasfresh/issues/3353) Implement MSV3 availability query
    * New vertical Feature for the Pharma Industry. Now it's able to do MSV3 Queries to vendors via metasfresh.
  * [#3354](https://github.com/metasfresh/metasfresh/issues/3354) Different subscription Receiver for ever
  * [#3355](https://github.com/metasfresh/metasfresh/issues/3355) Add option to automatically credit open invoice for terminated contract / subscription
  * [#3359](https://github.com/metasfresh/metasfresh/issues/3359) User Window unlock Account Action
    * Adding new Action in User Window in WebUI allowing to unlock the User Account.  
  * [#3366](https://github.com/metasfresh/metasfresh/issues/3366) Webui Window: Create window for ReferenceNo and Reference Type
    * New Windows for Reference No and Reference No Type maintenance.
  * [#3377](https://github.com/metasfresh/metasfresh/issues/3377) Add an ID to C_ReferenceNo_Type_Table
    * Improvement of the Reference No Type Table, now having a Primary Key.
  * [#3387](https://github.com/metasfresh/metasfresh/issues/3387) WebUI New Window for MSV3 Config
    * New Configuration Window in WebUI for MSV3 Connections to vendors in german Pharma Industry.
  * [#3385](https://github.com/metasfresh/metasfresh/issues/3385) Enlarge column AD_EntityType.EntityType
    * Resizing the Field entitytype from 40 to 512 chars.
  * [#3389](https://github.com/metasfresh/metasfresh/issues/3389) Performance issue related to zooming table record references
    * Improved Performance for table record references.
  * [#3416](https://github.com/metasfresh/metasfresh/issues/3416) Save termination date explicitly

* metasfresh-webui-api
  * [#744](https://github.com/metasfresh/metasfresh-webui-api/issues/744) Support Export of massive records to Excel
    * Improved Functionality of Excel Export, now allowing to export all selected records via main grid view and action menu entry.
  * [#766](https://github.com/metasfresh/metasfresh-webui-api/issues/766) Precision Layout in Price of Orderlines
    * New Precision Functionality in WebUI, now allowing to record and display more that 2 digits in precision.
  * [#772](https://github.com/metasfresh/metasfresh-webui-api/issues/772) EMail Attachment Name in WebUI
    * Improvement of the eMail Attachment Name in WebUI eMail editor, now showing the Documenttype and Documentno as combined attachment Name.
  * [#785](https://github.com/metasfresh/metasfresh-webui-api/issues/785) Act gracefully on old/invalid AD_UserQuery
    * Improvement of the User Query Handling. Now allowing the WebUI to ract on old/ incompatible Queries instead of failing.
  * [#788](https://github.com/metasfresh/metasfresh-webui-api/issues/788) Allow Filtering of Label-Type-Fields in WebUI
    * New Functionality that allows to add Label Type Fields in WebUI as Filter criteria.
  * [#793](https://github.com/metasfresh/metasfresh-webui-api/issues/793) Provide "loadDuration" when fetching document references
    * Internal Housekeeping improvement. Now providing the loadDuration of Document References in WebUI.
  * [#794](https://github.com/metasfresh/metasfresh-webui-api/issues/794) Provide actions evaluateDuration
    * Internal Housekeeping improvement. Now providing the evaluateDuration of Actions in WebUI.
  * [#798](https://github.com/metasfresh/metasfresh-webui-api/issues/798) Allow Filtering for Table References and show table identifier
    * New Feature in Labels widget. Now allowing to add and use Table references instead of reference lists. Also possible to add Label to Filter list.
  * [#813](https://github.com/metasfresh/metasfresh-webui-api/issues/813) Reduce Export Time for massive Exports

* metasfresh-webui-frontend
  * [#1252](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1252) Select all x items shall not be available when there is only one page of entries
    * Improved Handling of the select all functioanlity in Grid View. Now only showing toggle option when more than 1 page.
  * [#1502](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1502) Missing PropTypes Validation for noLabel isOpenDatePicker
    * Internal Housekeeping Issue. Adding PropType Validation for isOpenDatePicker.
  * [#1504](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1504) Make a difference between internal date format (ISO) and user friendly locale date
    * Improved Handlign of Date Widget reponses. Now distiguishing between Date for API and Date presented to the user.
  * [#1509](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1509) Harmonize details calendar widget with daterange widget in Filter
    * Improving the Layout of Date Picker, harmonizing with the look and feel of Date Range Widget.
  * [#1514](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1514) Filter Dropdown dynamically extend height when dropdown list selected
    * Improved Dropdown behavior. Now showing a complete dropdown List in Filters also when at the bottom of a Filter list area.
  * [#1428](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1428) Calendar icon covers date field
    * Refining the look and feel of the calendar icon behavior in WebUI grid views.

## Fixes
* metasfresh
  * [#1196](https://github.com/metasfresh/metasfresh/issues/1196) Creating new product in new database causes error
    * Fixes the sequence for M_Product Values on new Database seeds.
  * [#3196](https://github.com/metasfresh/metasfresh/issues/3196) Dunning run: Exception on PDF generation
    * Fixes the Dunning Run Action. Now the automatic PDF Generation works smoothly again.
  * [#3339](https://github.com/metasfresh/metasfresh/issues/3339) Field "Doctype" is included twice in payment window
    * Fixes a doubled Field for Doctype in the payment window.
  * [#3350](https://github.com/metasfresh/metasfresh/issues/3350) Error creating movement from DDOrder
    * Fixes an Error that prevented the creation of movements from Distribution Orders.
  * [#3386](https://github.com/metasfresh/metasfresh/issues/3386) Issued HUs retain I status after PP_Order unclose
  * [#3426](https://github.com/metasfresh/metasfresh/issues/3426) Dunning Level is not set in invoice after generating dunning doc

* metasfresh-webui-api
  * [#775](https://github.com/metasfresh/metasfresh-webui-api/issues/775) Destroyed HUs are still visible in material receipt
    * Destroyed HU are not shown in Handling Unit Editor anymore during the Material Receipt workflow.
  * [#777](https://github.com/metasfresh/metasfresh-webui-api/issues/777) Date and time filter: truncate to Day when filtering
    * Improvement of the Filter with Field format DateTime, now Truncating to Date when filtering.
  * [#781](https://github.com/metasfresh/metasfresh-webui-api/issues/781) HU editor view gets empty after splitting out one TU
    * Now showing the newly split Transportation Unit in Handling Unit Editor after transform.
  * [#786](https://github.com/metasfresh/metasfresh-webui-api/issues/786) Follow up destroyed HUs are still visible in material receipt
    * Hiding destroyed Handling Units in Material Receipt.
  * [#787](https://github.com/metasfresh/metasfresh-webui-api/issues/787) Deadlocks occurring around material cockpit
    * Fixes some deadlocks that occurred through Material Cockpit logic.
  * [#796](https://github.com/metasfresh/metasfresh-webui-api/issues/796) Error on filter with +/- buttons
    * Fixes an error that occurred when using the new DateSwitcher Widget.
  * [#803](https://github.com/metasfresh/metasfresh-webui-api/issues/803) NPE in Picking Tray Clearing
    * Fixes a Null Pointer Exception that ocurred under certain circumstances in Picking Tray Clearing Window in WebUI.
  * [#804](https://github.com/metasfresh/metasfresh-webui-api/issues/804) Error in Picking Tray Clearing when adding to existing HU
    * Fixes an Error that occurred in Picking Tray Clearing after adding to an existing Handling Unit.

* metasfresh-webui-frontend
  * [#1447](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1447) Picking window broken
    * Fixes the Picking Terminal Picking Slot View. Now showing the proper information about the Picking Slot Content and Businesspartner reservation.
  * [#1494](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1494) Picking Tray Clearing window: fix: Warning: Failed prop type: Invalid prop `selected` of type `string` supplied to `DocumentList`, expected `array`
    * Fixes the props validation in Picking Tray Clearing Window.
  * [#1495](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1495) Error on "add to transportation order"
    * Fixes a Bug that occurred in window Picking Tray Clearing when adding an HU to a Transportation Order.
  * [#1498](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1498) Frontend subscriptions to api's view topic get out of hand
    * Reducing the subscription amount per view, allowing to reduce the websocket connections "overload" on server side.
  * [#1508](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1508) Scrollbar in Filter when hovering apply Button
    * Improvement of the Tooltip Layout for Apply Button in Filter Selection Dropdowns.
  * [#1517](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1517) Discard changes in modal window
    * Fixes the discard of incomplete rows because of not filled mandatory fields.
  * [#1518](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1518) Create purchase orders: error in console
    * Fixes a Bug that prevented the creation of Purchase orders from Sales Orders to be done without errors.
  * [#1520](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1520) Typeahead error in new Label Filter
    * Fixes a Typeahead error in the new Label Filter in WebUI.
  * [#1529](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1529) Email To field does not work correctly
    * Improves the mailTo Field in WebUI. Now showing the Username instead of the user ID.
  * [#1536](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1536) Cannot set attributes in orderline
  * [#1552](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1552) Selecting country in dropdown with mouse click not possible

# metasfresh 5.41 (2018-03)
**release for week 2018-03**

## Features
* metasfresh-app
  * [#3209](https://github.com/metasfresh/metasfresh/issues/3209) Material Receipt candidates action for batch serial No on selected HU
    * New Action added for Serial No generation in Material Receipt and distribution to its received Handling Units.
  * [#3213](https://github.com/metasfresh/metasfresh/issues/3213) New Action for Repost Document in Accounting Transaction Window
    * New Action in Accounting Transaction Window, allowing to repost the shown lines.
  * [#3245](https://github.com/metasfresh/metasfresh/issues/3245) Material Cockpit Details modal overlay
    * Improvement for Material Cockpit, now allowing a modal overlay with detailed information about reserved and ordered quantities and their documents.
  * [#3271](https://github.com/metasfresh/metasfresh/issues/3271) Implement event log
    * New Event Log Functionality that is used first time for nearly realtime Material Cocpit updates.
  * [#3279](https://github.com/metasfresh/metasfresh/issues/3279) Pharma: Copy missing product prices after import
    * New Functionality after import of pharmaceutlical prodcuts. Now automatically creating product prices in the corresponding pricelist versions.
  * [#3284](https://github.com/metasfresh/metasfresh/issues/3284) Translation of eMail Editor in WebUI
    * Translation of the eMail Editor in WebUI for Language/ Locale de_DE.
  * [#3286](https://github.com/metasfresh/metasfresh/issues/3286) Workaround for truncating T_WEBUI_ViewSelection/-Line
    * Temporary Solution for the data growth of ViewSelection and ViewSelectionline tables.
  * [#3288](https://github.com/metasfresh/metasfresh/issues/3288) Shipper Transportation: Shipper Location: change validation rule logic
    * Adjustment of the Shipper Transportation validation rule logic.
  * [#3289](https://github.com/metasfresh/metasfresh/issues/3289) WebUI: New Window for Document Details in Material Cockpit
    * New Window for Document Details that can now be shown via Material Cockpit Window.
  * [#3293](https://github.com/metasfresh/metasfresh/issues/3293) WebUI: Add Translation Messages for Daterangepicker
    * Improved Translations. Added static translations for de_DE, en_US and Date Range Picker.
  * [#3303](https://github.com/metasfresh/metasfresh/issues/3303) WebUI: New Window for GO! Delivery Orders
    * New Window in WebUI for the new Functionality of General Overnight Shipper Transportation.
  * [#3304](https://github.com/metasfresh/metasfresh/issues/3304) Copy C_DocType.Description/DescriptionBottom to Order and Invoice
    * New feature for Documents Generation. Now it's possible to define default text snippets in Document Types and copy these automatically to the created document description when selecting the Document type.
  * [#3309](https://github.com/metasfresh/metasfresh/issues/3309) WebUI Window Design: Improve window Event store
    * New System Admin Window Event Store. Allows the System Admin to view the status of events and checking/ resubmitting them in case of issues.

* metasfresh-webui-API
  * [#672](https://github.com/metasfresh/metasfresh-webui-api/issues/672) Window for easy Distribution Orderlines Handling in WebUI
    * New Window that allows the Handling of Distribution Orderlines in WebUI.
  * [#737](https://github.com/metasfresh/metasfresh-webui-api/issues/737) Deal properly with T_WEBUI_ViewSelection[Line]
    * Improvement of WebUI temporary selections.
  * [#745](https://github.com/metasfresh/metasfresh-webui-api/issues/745) Batch entry mode w/o Packing Instruction branch:master type:enhancement
    * Improvement of the Batch entry mode functionality. Now it's possible to configure the Batch entry via Sysconfig so that no Packing Instruction is needed for recording.
  * [#762](https://github.com/metasfresh/metasfresh-webui-api/issues/762) Show onhand quantity in new WebUI MRP Product Info Window
    * New Field in material Cockpit, now showing the on Hand Quantity too.
  * [#770](https://github.com/metasfresh/metasfresh-webui-api/issues/770) Raise session Timeout of WebUI Application
    * Now possible to configure the session timeout of metasfresh via Spring Boot.
  * [#778](https://github.com/metasfresh/metasfresh-webui-api/issues/778) Use readOnlyFlag from AD_Field and AD_Tab when creating DocumentLayoutElements
    * Improvement of the Read-Only functionality in WebUI, now respecting the configuration doen in AD_Fields and AD_TAB about the readOnly Flag.

* metasfresh-webui-frontend
  * [#1470](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1470) Bug in long texts with new line
    * Improving the behavior in LongText Fields. Now only patching the content when leaving the Field.
  * [#1478](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1478) Attachment in eMail Editor: Show File name/ caption instead of key
    * Improving the Names for attached Files in eMail Editor. Now showing the caption names instead of attachment keys.
  * [#1485](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1485) Tooltip for for "Select all"/ "Select all x rows"
    * New Tooltip for the Select All Functionality.

## Fixes
* metasfresh-app
  * [#3232](https://github.com/metasfresh/metasfresh/issues/3232) Disposal creates Invoice Candidates
    * Improved Feature, now possible to prohibit the creation of Invoice Candidates in Disposal Workflow.
  * [#3291](https://github.com/metasfresh/metasfresh/issues/3291) Search Icon disappears when switching Main-Subtab in Contract Window
    * Fixes the vanishing Search Icon in window contracts of metasfresh swingUI.

* metasfresh-webui-frontend
  * [#1348](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1348) Keeping lines selected when turning the page not working
    * Fixes the Pagination after selecting lines. Now the selections are kept when switching pages.
  * [#1429](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1429) Left and right key doesn't work on date edit field
  * [#1481](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1481) Cannot open "Create purchase orders" modal view
    * Now enables to open modal overlays from action menu again.

# metasfresh 5.40 (2018-02)

**release for week 2018-02**

## Features
* metasfresh-app
  * [#1752](https://github.com/metasfresh/metasfresh/issues/1752) System Element overwrite on Window Field
    *  New Feature in the Application Dictionary, now able to overwrite the system element on Field Level.
  * [#3155](https://github.com/metasfresh/metasfresh/issues/3155) Create special pharma import product table
    * New vertical Feature for the import of products from pharma industry.
  * [#3222](https://github.com/metasfresh/metasfresh/issues/3222) Refactor trx event listeners
    * Improvement of Transaction event listeners, now leading to explicit specification which code shall be executed on which event.
  * [#3229](https://github.com/metasfresh/metasfresh/issues/3229) Show c_activity_ID in purchase Orderlines Grid View
    * New Field for Activity in Purchase Orderlines.
  * [#3234](https://github.com/metasfresh/metasfresh/issues/3234) Material Tracking ID in Invoice Candidates Filter shall be search
    * Improving the Material Tracking ID Lookup widget. It is now an autocomplete search field instead of a dropdown list.
  * [#3237](https://github.com/metasfresh/metasfresh/issues/3237) New Document "Source of Supply"
    * Improvement of the shipping workflow, now also able t create a "Source of Supply" Document for the shipped Products.
  * [#3238](https://github.com/metasfresh/metasfresh/issues/3238) Create Missing M_Cost records on the fly
    * Improvement of the M_Cost handling, now creating missing entries on the fly.
  * [#3230](https://github.com/metasfresh/metasfresh/issues/3230) Pharma: import prices
    * New Import Prices functionality for products from pharma industry.
  * [#3239](https://github.com/metasfresh/metasfresh/issues/3239) WebUI: Material Receipt Candidates Fields not readonly
    * Improvement of the Material Receipt Candidates Window in WebUI. Now Fields are readonly that should not be changes by the user after creation.
  * [#3242](https://github.com/metasfresh/metasfresh/issues/3242) WebUI: Create new Customer Accounts Window
    * New Window for Customer Accounts, allowing the user to define customer relevant accounting information.
  * [#3243](https://github.com/metasfresh/metasfresh/issues/3243) WebUI: Adjust the BOM Configuration window in Subtab for components
    * Improvement of the BOM Configuration Window and Forumula. Now showing most important columns in grid view for components. Renaming Fields and translations for better understanding.
  * [#3255](https://github.com/metasfresh/metasfresh/issues/3255) WebUI: Accounting Schema Window
    * New Window in WebUI for Accounting Schema, allowing the user to maintain the default Accounting properties.
  * [#3256](https://github.com/metasfresh/metasfresh/issues/3256) WebUI: Window for Warehouse Accounting
    * New Window for Vendor Accounts, allowing the user to define warehouse relevant accounting information.
  * [#3257](https://github.com/metasfresh/metasfresh/issues/3257) WebUI: Window for Vendor Accounting
    * New Window for Vendor Accounts, allowing the user to define vendor relevant accounting information.
  * [#3260](https://github.com/metasfresh/metasfresh/issues/3260) Hide Accounts Tab from Warehouse Window in WebUI
    * Hiding Accounts Tab in Warehouse Window, now available via Document Reference.
  * [#3261](https://github.com/metasfresh/metasfresh/issues/3261) WebUI: New Window for BPartner Group Accounts
    * New Window for Business Partner Group Accounts, allowing the user to define relevant accounting information for Business Partner Groups.
  * [#3267](https://github.com/metasfresh/metasfresh/issues/3267) WebUI: Add Create Periods to Action menu in Calendar Window
    * Improving the Calender and Period Window in WebUI, adding the Create Periods process to action menu.
  * [#3269](https://github.com/metasfresh/metasfresh/issues/3269) WebUI: Add Shortcut Filter from Calendar Year to Periods Window
    * Improving the Usability of Calendar and Period Window, now allowing to directly zoom to filtered Periods for a given year.
  * [#3272](https://github.com/metasfresh/metasfresh/issues/3272) Provide Periods for 2018
    * Housekeeping issue, providing the periods for 2018 as migration script.
  * [#3275](https://github.com/metasfresh/metasfresh/issues/3275) New Filter for datepromised in Sales/ Purchase Order
    * Adding the Filter for datepromised in Sales Order and Purchase order Window in WebUI.

* metasfresh-webui-api
  * [#752](https://github.com/metasfresh/metasfresh-webui-api/issues/752) Picking Tray Clearing: picking slot filter no results
    * Improvement of the filtering in Picking Tray Window. Now showing "No Rows" for en empty result instead of en Error message.
  * [#758](https://github.com/metasfresh/metasfresh-webui-api/issues/758) Picking Tray Clearing: process to take out an HU and add it to existing HU
    * New Functionality in Picking tray Clearing, having a new Action that takes out Handling Units from Picking Slot and adds to existing HU.
  * [#760](https://github.com/metasfresh/metasfresh-webui-api/issues/760) Picking Tray Clearing: process to take out an HU and add it to new HU
    * New Functionality in Picking tray Clearing, having a new Action that takes out Handling Units from Picking Slot and adds to a new HU.
  * [#763](https://github.com/metasfresh/metasfresh-webui-api/issues/763) Picking Tray Clearing: packing HUs: Add to Transportation Order, Ship and Invoice action
    * New Functionality in Picking tray Clearing, having a new Action that adds Handling Units to Transportation order and automatically creates Shipments and Invoiced for the HU.
  * [#764](https://github.com/metasfresh/metasfresh-webui-api/issues/764) Receipt candidates: HU editor: cannot call Transform for a CU
    * Improvement of Receipt Candidates, now allowing to transform Customer Units.
  * [#768](https://github.com/metasfresh/metasfresh-webui-api/issues/768) Picking Tray Clearing: packing HUs: generate shipper's package label
    * New Functionality in Picking tray Clearing, generating a shipper package Label for package HU.
  * [#769](https://github.com/metasfresh/metasfresh-webui-api/issues/769) New context variable for isWebUI
    * Improvement of Display logic in WebUI now allowing to use "isWebUI" flag in display logic.

* metasfresh-webui-frontend
  * [#1465](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1465) frontend: Processes: when calling a process frontend shall provide which are the selected rows in the left/right view
    * Enhanced funcktionality in WebUI selectedIDs. Now it's possible to select lines in splitted views so that actions/ process receive all selected Ids.
  * [#1475](https://github.com/metasfresh/metasfresh-webui-frontend/issues/1475) Hover showing Element Content for flags wrongly
    * Improvement of the tablecell tooltips in Grid Views. Not not showing a tooltip for checkboxes and switches anymore.

#Fixes
* metasfresh-app
  * [#2822](https://github.com/metasfresh/metasfresh/issues/2822) Empty Country in Price List not working
    * Fixes the price retrieval Logic for Pricelists with empty country.
  * [#3225](https://github.com/metasfresh/metasfresh/issues/3225) Error on unclosing a "manually" created PPOrder
    * Fixes a Bug that appeared when trying to manually unclose a Manufacturing Order.
  * [#3227](https://github.com/metasfresh/metasfresh/issues/3227) Attachment related perf problem in swing client
    * Fixes a Performance Issue that was related to missing indices in Attachment.
  * [#3233](https://github.com/metasfresh/metasfresh/issues/3233) WebUI: Role permission constraints missing in Subtabs
    * Fixes an issue that allowed to add duplicate permissions in WebUI Role Window.
  * [#3281](https://github.com/metasfresh/metasfresh/issues/3281) C_Tax.ValidFrom bug
    * Fix for the check of valid from date in Tax ID retrieval.

* metasfresh-webui-api
  * [#741](https://github.com/metasfresh/metasfresh-webui-api/issues/741) WebUI window C_Printing_Queue broken
    * Fixes the Prining Queue Window in WebUI.
  * [#757](https://github.com/metasfresh/metasfresh-webui-api/issues/757) elasticsearch shall use slf4j instead of log4j
    * Switches the logger for elasticsearch to slf4j.


