## Create a Subaccount and entitle Kyma Runtime

SAP BTP, Kyma runtime provides a fully managed Kubernetes runtime based on the open-source project "Kyma". With this cloud-native solution, developers can extend SAP solutions with serverless Functions and combine them with containerized microservices.

### Create a Subaccount

In a BTP **Enterprise Account** training environment, create a new subaccount for this tutorial. <br>

In a BTP **Trial Account**, a subaccount with Kyma entitlement is already preconfigured. You can create a 2nd Subaccount in Trial also, but you will not have unused entitlements for Kyma. You need to delete the Kyma entitlement in the preconfigured Subaccount first.

**Procedure**

1. Naviagte to your **Global Account Account Explorer**, quasi the home page of your GA. <br>
   Select **Create --> Subaccount**.
   
   ![](images/22_1_createsub.png)

2. Prvoide a **Name** and your preferred **Region**.  <br>
   For more details about Regions where Kyma is available, see [Discovery Center](https://discovery-center.cloud.sap/serviceCatalog/kyma-runtime?region=all). <br>
   You may also change the **Subdomain**, however there is no reason in thsi turorial. <br> 
   Note: The subdomain will become part of the URL for accessing applications that you subscribe to from this subaccount. 
   The subdomain must be unique across all subaccounts in the same region. Uppercase and lowercase will not differentiate subdomains.

   ![](images/22_2_createsub.png)

3. The Subaccount will be created.

   ![](images/22_3_createsub.png)

4. Enter your subaccount and 

   ![](images/22_4_entersub.png)

5. scroll down to **Entitlements**.
   The preconfigured services are shown.
   
<br>

### Entitle Kyma Runtime

If you use a BTP Trial Account, you are already entitled to use the **Kyma runtime** Service. 
If you use a BTP Enterprise Account, you are not yet entitled to for the **Kyma runtime** Service. 


**Procedure**

1. In your subaccount, navigate to **Entitlements --> Entity Assignments**. <br>
   Select Entity **YourSubaccount** of choice. <br>
   Put **Kyma** into the searchfield. <br>
   And press button **Configure Entitlements**. <br>

   ![](images/2_1_kyma_entitlement_1.png)

2. The buttons will change. Select **Add Service Plan**.

   ![](images/2_2_kyma_entitlement_2.png)

3. A pop-up window will come up. <br>
   Search for **Kyma** in "All Solutions". <br>
   Select **Kyma Runtime**. <br>
   And select your **Service Plan** of choice.  <br>
   Press **Add 1 Service Plan**.  <br>

   ![](images/2_3_kyma_addsplan_1.png)

4. Increase optionally your "Subaccount Assignment". For training keep "1".
   Press **Save**

   ![](images/2_4_kyma_addsplan_2.png)

5. Your entitlements will be saved.

   ![](images/2_4_kyma_addsplan_3.png)

6. Double-check your entitlements when done:

   ![](images/2_5_kyma_entitled.png)

