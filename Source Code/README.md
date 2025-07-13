# 🚀 How to Use/Import
To utilize these solutions, you will need to import them into your Power Platform environment.

## Prerequisites:
- Access to a Power Platform environment (e.g., Dataverse, Power Apps, Power Automate).
- Sufficient permissions to import solutions within that environment.

## Steps to Import an Unmanaged Solution:
- **Download the Solution:** Navigate to this source-code folder in the GitHub repository and download the desired .zip solution file to your local machine.
- **Access Power Apps Maker Portal:** Go to [make.powerapps.com](https://make.powerapps.com).
- **Select Environment:** Ensure you are in the correct Power Platform environment where you intend to import the solution. You can change environments using the environment selector in the top right corner.
- **Navigate to Solutions:** In the left-hand navigation pane, click on "Solutions".
- **Navigate to Solutions:** In the left-hand navigation pane, click on "Solutions".
- **Upload File:** In the "Import a solution" pane, click "Browse" and select the .zip file you downloaded.
- **Next & Import:** Follow the on-screen prompts, click "Next", and then "Import".
- **Monitor Import:** The import process may take a few moments. You will receive a notification upon successful completion.


> Please refert to Microsoft's **[reference](https://learn.microsoft.com/en-us/power-apps/maker/data-platform/import-update-export-solutions)** on how to import solution in Power Platform environment.


# ⚠️ Important Considerations for Unmanaged Solutions
- **Unmanaged Nature:** These are unmanaged solutions. When an unmanaged solution is imported, all its components are added directly to your environment. They become part of the environment's default solution and can be individually modified or deleted.
- **Development Environments:** It is highly recommended to import these solutions into a development or sandbox environment first. Avoid importing unmanaged solutions directly into production environments unless you fully understand the implications and have a robust deployment strategy.
- **Component Overwrite:** If components with the same unique name already exist in your environment, importing an unmanaged solution will overwrite them. Exercise caution.
- **No Dependency Tracking (for updates):** Unlike managed solutions, unmanaged solutions do not maintain a direct link to their source after import. If you import a newer version of an unmanaged solution, it will add/update components, but it won't automatically remove components that were in the previous version but are no longer in the new one. Manual cleanup might be required for deprecated components.

# 🛠️ Best Practices
- **Version Control:** This repository serves as the version control for these solutions. Always ensure you are working with the latest version from this repository.
- **Environment Strategy:** Implement a clear environment strategy (e.g., Dev -> Test -> Prod) and use appropriate solution types (unmanaged for Dev, managed for Test/Prod) for your deployment pipeline.
- **Power Platform CLI:** For advanced users and automated deployments, consider using the **[Power Platform CLI](https://learn.microsoft.com/en-us/power-platform/developer/cli/introduction)** to export and import solutions programmatically.

# 💬 Feedback and Contributions
If you encounter any issues with these solutions, have suggestions for improvements, or wish to contribute, please feel free to reach out or open a new issue on the GitHub repository.

