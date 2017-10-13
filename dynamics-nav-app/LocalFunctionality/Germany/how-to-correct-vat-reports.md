---
    title: How to Correct VAT Reports 
    description: If you have to submit a corrective VAT report or delete a submitted VAT report, you must create a new VAT report. According to the legislation, a corrective report must be submitted within a month of the initial report.
    services: project-madeira
    documentationcenter: ''
    author: SorenGP

    ms.prod: "dynamics-nav-2017"
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 07/01/2017
    ms.author: sgroespe

---
# How to: Correct VAT Reports
If you have to submit a corrective VAT report or delete a submitted VAT report, you must create a new VAT report. According to the legislation, a corrective report must be submitted within a month of the initial report.  
  
 When you create a corrective report, the report will contain two line types per corrected line. In one line type, Cancellation, the base value of the VAT is reported as a cancellation. All other information remains the same, and cannot be edited. On a new line, Correction type, you can make corrections as needed to the VAT amount. The **Suggest Lines** action, however, will suggest the correct amount based on the filters and posted documents. You cannot correct or modify the **VAT Registration No.** Each period being corrected needs its own corrective report.  
  
 The **Suggest Lines** action recalculates the values to report. The **Correct Lines** action is used to make manual changes. You can combine the effects of the two actions to correct your report.  
  
 **Example corrections scenarios**  
  
1.  If you post additional VAT entries after you submit the Standard report in the report period, choose **Suggest Lines** in the **Process** group to get the updated amounts.  
  
    > [!NOTE]  
    >  If you manually changed the amount for a customer or vendor, this amount will be overwritten when additional VAT entries are posted. Update the amount accordingly.  
  
2.  If you want to change the amount of a report line that has already been submitted and no new VAT entries are posted, choose **Correct Lines** in the **Process** group. The **VAT Report Lines** window opens. Select the lines that you want to correct. Choose the **OK** button.  
  
     For each entry, two lines are displayed: Cancellation and Correction. You can now change the amount on the Correction line.  
  
    > [!NOTE]  
    >  The **Correct Lines** action will not suggest the amount based in VAT entries. If you have new VAT entries for the customer or vendor, instead use **Suggest Lines**.  
  
3.  If you used the wrong filters, for example, the wrong VAT Product Posting Group, choose **Suggest Lines** in the **Process** group and set the filters as needed.  
  
     **Suggest Lines** will create entries to account for the difference between the filters.  
  
    > [!NOTE]  
    >  If the updated filters exclude a customer or vendor, [!INCLUDE[navnow](../../includes/navnow_md.md)] creates a Cancellation line for the previous reported amount and a Correction entry with amount 0.  
  
### To correct a VAT report  
  
1.  Create a new VAT report. For more information, see [How to: Create VAT Reports](how-to-create-vat-reports.md).  
  
2.  Fill in the fields in the **General** FastTab, and set the **VAT Report Type** field to Corrective.  
  
3.  In the **Original Report No.** field, select the report that you want to correct. You can only select reports of type Standard that have been marked as Submitted.  
  
4.  Create your correction VAT Report Line entries.  
  
     On the **Actions** tab, choose **Suggest Lines**. Set the filters as needed.  
  
     On each line you can drill down on the amounts to see which VAT entries make up the amount. Change the amount if needed. You cannot edit, however, the **VAT Registration No.**.  
  
5.  If the **Suggest Lines** action does not provide suggestions to correct the amounts that you intended, use the **Correct Lines** action to insert Cancellation and Correction lines for the customer or vendor.  
  
6.  Continue with the VAT report creation process, and release the report.  
  
## See Also  
 [How to: Set Up VAT Reports](how-to-set-up-vat-reports.md)