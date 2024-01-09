---
layout: default
title: Mvp
nav_exclude: true
---

### **Web Application Components Overview**

Our web application boasts an intelligent design, segmented into four key components: the Input Box, Dynamic Area, Overview, and Output Message. Each is meticulously crafted to maximize user experience and efficiency.

#### **1. Input Box**



-   **Function**: Enables users to issue commands in a natural, intuitive language.
-   **Ease of Use**: Commands mirror everyday language, making the system accessible and user-friendly.
-   **Command Submission**: Simply press 'Enter' to send commands for processing.

#### **2. Output Message**


-   **Immediate Feedback**: Offers real-time, single-line feedback for each command.
-   **Color-Coded Clarity**: Green for success, red for errors.
-   **Error Resolution**: Identifies mistakes and suggests correct usage in case of an error.

#### **3. Dynamic Area**



-   **Interactive Canvas**: Visualize data through Table or Plot objects.
-   **Contextual Command Suggestions**: Provides relevant command suggestions based on user activity.
-   **Automatic Layout Management**: Intuitively arranges visualizations for optimal display and analysis, enhancing the user’s experience in data handling and interpretation.

#### **4. Overview**

-   **Data Management**: Displays all available Tables and Plots for easy tracking and access.
-   **Organized Analysis**: Facilitates an organized and efficient approach to data visualization.

Each component is designed with a focus on intuitive use, efficiency, and user-friendly interfaces. Our application is not just a tool, but a comprehensive solution that we believe will exceed the expectations of our investors and users.

### **Getting Started with the Application: Basic Usage**

This section guides you through the fundamental operations of our web application, detailing the process of importing and exporting datasets. Our aim is to ensure a smooth and straightforward experience for all users, even those new to the platform.

#### **1. Importing Datasets**

-   **Command**: Type `import` in the Input Box and press 'Enter'.
-   **Function**: A popup will appear, allowing you to upload your datasets.
-   **Data Type**: Initially, the app supports only Time-Series Data.
-   **Flexibility in Format**: The app is equipped with a robust import-export module capable of handling various data formats. This module seamlessly transforms any format into a compatible one, ensuring smooth integration into the system.

#### **2. Exporting Data**

-   **Command**: Use the command `export [name]`, replacing '[name]' with the specific name of the plot or table you wish to download.
-   **Function**: Executing this command will trigger an automatic download of the chosen plot or table.

Our platform's intuitive design and powerful import-export capabilities make it an ideal tool for efficient data management. Whether you're importing various data formats or exporting your analytical results, the process is designed to be as straightforward and user-friendly as possible.

### **Viewing and Managing Data**

After successfully importing datasets into the system, users can effortlessly view and manipulate their data within the Dynamic Area. This section outlines the commands for displaying and removing datasets, ensuring a seamless interaction with the system.

#### **1. Displaying Data**

-   **Command**: Enter `show [name]` in the Input Box, replacing '[name]' with the dataset's name.
-   **Function**: This command will load the named dataset into the Dynamic Area, displaying it as a table.
-   **User Experience**: The data is presented in an organized and readable table format, allowing for easy analysis and interpretation.

#### **2. Removing Data from View**

-   **Command**: Use `remove [name]`, substituting '[name]' with the dataset's name.
-   **Function**: This will remove the named dataset from the Dynamic Area.
-   **Data Integrity**: Removing a dataset from view does not delete it from the system; it merely clears the display, ensuring data is safely stored for future use.

The ability to display and remove datasets with simple commands enhances the application's usability. These features are designed to provide users with a flexible and efficient way to interact with their data, catering to both beginners and advanced users alike.

### **Data Cleaning Functionalities**

Our application provides robust data cleaning capabilities, essential for maintaining data quality and integrity. Below are the adapted commands tailored to fit the intuitive design of our current project.

#### **1. Removing Duplicates**

-   **Command**: `remove duplicates [name]`
-   **Function**: This command eliminates all duplicate entries from the dataset named '[name]'.

#### **2. Handling Missing Values**

-   **Command**: `handle missing [name] [method]`
    -   If no method is specified, the system employs a default mean imputation.
-   **Common Methods**:
    -   **Mean Imputation**: Replaces missing values with the mean of the column.
    -   **Median Imputation**: Substitutes missing values with the median of the column.
    -   **Mode Imputation**: Fills missing values using the mode.
    -   **Forward/Backward Fill**: Propagates the next or previous value to fill gaps.

#### **3. Column Management**

-   **Keep Specific Columns**:
    -   **Command**: `keep columns [name] [column1],[column2]`
    -   **Function**: Retains only the specified columns in the named dataset.
-   **Remove Specific Columns**:
    -   **Command**: `remove columns [name] [column1],[column2]`
    -   **Function**: Deletes the specified columns from the named dataset.

#### **4. Row Management**

-   **Keep Specific Rows**:
    -   **Command**: `keep rows [name] [row1],[row2]`
    -   **Function**: Preserves only the specified rows in the named dataset.
-   **Remove Specific Rows**:
    -   **Command**: `remove rows [name] [row1],[row2]`
    -   **Function**: Eliminates the specified rows from the named dataset.

These commands are designed to offer a straightforward and efficient approach to data cleaning, ensuring users can easily optimize their datasets for analysis.

### **Data Visualization Functionalities**

Our application supports a variety of data visualization formats, allowing users to create and manipulate line graphs, pie charts, bar charts, and scatterplots. Here’s how users can utilize these features:

#### **1. Creating Plots**

-   **Command**: `create [plottype] [name]`
-   **Function**: Adds an empty plot of the specified type (line graph, pie chart, bar chart, scatterplot) to the Dynamic Area and to the plots section, named '[name]'. The plot will have a '*' after its name to indicate it is not yet saved.

#### **2. Line Graph**

-   **Command**: `load into [name] from [table name] [row names]`
-   **Function**: Plots values from specified rows over time, creating a line graph where each line represents a unique row, ideal for comparing trends across different categories over time.

#### **3. Bar Chart**

-   **Command**: `load into [name] from [table name] [column name]`
-   **Function**: Visualizes values for each record in the specified column as a bar chart, useful for displaying time series data where each column represents a different time point.

#### **4. Pie Chart**

-   **Command**: `load into [name] from [table name] [column name]`
-   **Function**: Displays the distribution of data in the specified column using a pie chart, offering a clear visual representation of data segments.

#### **5. Scatterplot**

-   **Command**: `load into [name] from [table name] [x-axis column name], [y-axis column name]`
-   **Function**: Creates a scatterplot by plotting data points based on values in the specified x-axis and y-axis columns, useful for identifying patterns and relationships between two variables.

These visualization tools are designed to provide insightful and clear representations of your data, aiding in analysis and decision-making.

### **Finalizing and Managing Your Visualizations**

In the last segment of our guide, we cover the crucial steps of saving changes and deleting visualizations, ensuring that your work is securely stored or removed as needed.

#### **1. Saving Changes**

-   **Command**: `save [name]`
-   **Function**: This command updates the system with any changes made to the plot or table named '[name]'. Once saved, the asterisk (*) indicating an unsaved state is removed, signifying that your work is securely stored within the system.

#### **2. Deleting Visualizations or Data**

-   **Command**: `delete [name]`
-   **Function**: Use this command to permanently remove the named plot, table, or dataset from the system. It’s an irreversible action that helps in managing and organizing your workspace by eliminating unnecessary or outdated items.

By using these commands, you can effectively manage your work, ensuring that your visualizations and data are current and organized. Remember, the 'save' command solidifies your changes, while the 'delete' command clears items from your workspace, making room for new analyses and visualizations.
