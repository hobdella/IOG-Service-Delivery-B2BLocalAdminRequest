# IOG-Service-Delivery-B2BLocalAdminRequest

**Overview**

This service exists to allow end users to request local admin rights on their assigned workstation/laptop/virtual machine. The process falls into 3 main parts, the user's request, the approval stage and provisioning the local admin access if applicable.

**Process**

**The User Request**
The user requests local admin from the ITSM platform self-service form, the request must include busieness justification for the request including a scope of what would be considered insufficient levels of detail. A preliminary reqeust for change is created and is sent automatically to the user's manager for approval. The manager must approve the pRFC before it will proceed to the approval stage in Service Delivery.

**The Service Delivery Approval**
The request is received into the a defined group of approvers and a review of the request is made. There are a generally understood basis for the approving or rejecting of requests and the approval can take the form or permanent or temporary rights being granted, or rejection. The approver makes their decision and updates the ticket accordingly. A rejected request will usually direct the user to contact IT support as a one-off need is handled by elevated rights on a remote support session. Approved rights will see the request excalated to the InfoSec Access Management team for applying the rights.

**Provisioning Local Admin Rights**
The user is added to the local admin users group in Active Directory for the taret device. 
The user is added to the RBI-GPO IT Users /BIN-GPO IT Users group depending on user's base location. (US=BIN, ROW=B2B)
The user is removed from the RBI-GPO Standard Users/BIN-GPO Standard Users
The user is sent confirmation admin rights have been granted and what steps to follow to have the rights apply.
The ticket is marked completed.
