## Create a Hello-World Kyma Function

Now, as the BTP Service Kyma is entitled and enabled, you can create the first service in Kyma.
In this card, you will use Kyma Dashboard to create a Kyma function. 
The other option is to use a Command Line tool, which we will cover later in this tutorial.

You cann follow this tutorial also on Kyma Docs, [Deploy and expose a Function](https://kyma-project.io/docs/kyma/latest/02-get-started/02-deploy-expose-function/) .

**Procedure**


1. Open your Kyma Dashboard (see previous card of the tutorial). <br>
   Choose **Namespaces** from the left-handed navigation. <br>
   Choose **default** in the Namesapces list or from the drop-down list-box. <br>
    
   ![](images/3_1_kyma_namespace.png)

2. In the default Namespace, select **Workloads --> Functions** and select **+ Create Function**.

   ![](images/3_2_kyma_function_1.png)

3. The "Create Function" wizard opens. Keep the preset **Simple**<br>
   Provide a name, e.g. **hello-world**. <br>
   Choose **Language** > **nodejs**. <br>
   Choose your **Runtime Version** > e.g. **node.js 16**. <br>
   Keep the preset values. Note that a YAML file will be created under **Source**.  <br>
   You may now also the check the other presets advanced and yaml.  <br>
   Choose **Create**

   ![](images/3_2_kyma_function_2.png)

4. The result is a new function **hello-world** in Kyma Functions.

   ![](images/3_2_kyma_function_3.png)

5. Navigate to **Discovery and Network --> API Rules**.  <br>
   Select **+ Create API Rule**.

   ![](images/3_3_kyma_api_1.png)
   
6. Provide a name, e.g. **hello-rule**
   As Service, choose the function you just created: **hello-world**.  <br>
   Keep the prefilled Gateway.  <br>
   You see that the **Host** defintion is incomplete.  <br>
   Provide a unique name for the host which is not yet in use. E.g. **hello-host**.   <br>
   Keep the **Rules** as is. <br>
   Choose **Create**.
      
   ![](images/3_3_kyma_api_3.png)

7. The API Rule "hello-rule" is created. <br>
   Click on the host URL to execute your funtion in a browser window.

   ![](images/3_3_kyma_api_4.png)
   
8. A browser windows will open showing the result of the function:

   **`Hello World from the Kyma Function hello-world running on nodejs16!`**
      
9. you may also execute your funtion under **Workloads --> Functions**. Select Function "hello-world". <br>
   Select **Configuration**
      
   ![](images/3_3_kyma_api_5.png)
