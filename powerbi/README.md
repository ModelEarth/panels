## **Title: Documentation for Pulling Supabase Data into Microsoft Power BI**

**Introduction**

This document provides a step-by-step guide on how to pull data from a Supabase database into Microsoft Power BI using the Supabase REST API. The objective of this process is to enable seamless data visualization and analysis within Power BI, using data stored in a Supabase database.

### **Step-by-Step Process**

### *Step 1: Access the Supabase REST API and Retrieve the Necessary API Key*

- **Objective**: Obtain the API key (anon key) and the correct URL for accessing the data in Supabase.
- **Instructions**:
    1. Log in to your Supabase project dashboard.
    2. Navigate to the **Settings** > **API** section.
    3. Note the base URL for your project and the anon key.

### *Step 2: Prepare the Supabase REST API Endpoint*

- **Objective**: Construct the API endpoint to retrieve data from the desired table or view in Supabase.
- **Instructions**:
    1. Identify the table or view you want to pull data from. For this example, we’re using the flow_impact_view.
    2. Construct the endpoint URL : <https://wovjoodfvamzysoxamdb.supabase.co/rest/v1/flow_impact_view>
    3. Since Power BI requires the API key to be passed in the URL, append the anon key as a query parameter.

### *Step 3: Open Power BI and Get Data from the Supabase API*

- **Objective**: Connect Power BI to the Supabase REST API and import the data.
- **Instructions**:
    1. Open **Microsoft Power BI Desktop**.
    2. Click on **Get Data** > **Web**.
    3. In the dialog box, paste the URL constructed in Step 2 into the **URL** field.
    4. Choose **Anonymous** as the authentication method, since the API key is embedded in the URL.
    5. Click **Connect** to load the data.

### *Step 4: Verify the Data in Power BI*

- **Objective**: Ensure that the data has been correctly imported into Power BI.
- **Instructions**:
    1. After connecting, Power BI will display a preview of the data.
    2. Verify that all the necessary columns and rows are present.
    3. Load the data into Power BI by clicking **Load**.

### **Sample Visualization**

Below is a bar chart visualization created in Microsoft Power BI using the data pulled from the Supabase flow_impact_view. The chart shows different emission types (Flowable) and their corresponding Flow Amount.

**Chart Title**: Emission Type by Flow Amount

<a href="img/barchart.png"><img src="img/barchart.png" style="width:100%;max-width:800px;"></a>

### **Conclusion**

You have successfully pulled data from a Supabase database into Microsoft Power BI using the Supabase REST API. The data is now ready for analysis and visualization within Power BI. This process can be repeated for other views or tables in Supabase as needed.