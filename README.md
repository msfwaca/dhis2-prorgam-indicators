# DHIS2 Program Indicators Repository

This repository contains the metadata configurations and scripts for **Program Indicators**. These program indicators are designed for tracking and monitoring health data within the DHIS2 system. Below are the steps to get started with cloning the repository, making necessary changes in the dev environment, and moving the updates to the test and production environments.

## Table of Contents
1. [Getting Started](#getting-started)
2. [Development Environment Setup](#development-environment-setup)
3. [Importing Metadata to DHIS2](#importing-metadata-to-dhis2)
4. [Testing Changes](#testing-changes)
5. [Promoting to Test and Production Environments](#promoting-to-test-and-production-environments)
6. [Contributing](#contributing)

## Getting Started

To start working on the DHIS2 program indicators, follow these steps to clone the repository and set up your local environment.

### Prerequisites
- Ensure you have Git installed.
- Access to a **DHIS2 instance** (Development, Test, and Production environments should be configured separately).

### Step 1: Clone the Repository

Open your terminal and run the following command to clone the repository:

```bash
git clone https://github.com/msfwaca/dhis2-program-indicators.git
cd dhis2-program-indicators
```
## Development Environment Setup

After cloning the repository, you need to configure your local DHIS2 environment where you will import the metadata. Follow these steps:

### Step 1: Import Metadata to DHIS2 Dev Environment

1. Log in to your DHIS2 development instance.
2. Navigate to **Import/Export App**.
3. Select **Metadata Import**.
4. Upload the appropriate metadata file from the cloned repository (`metadata.json` or other relevant files) to import it to the DHIS2 instance.
5. Review the import summary for any errors or warnings.

### Step 2: Make Necessary Changes

Once the metadata is successfully imported, you can begin editing program indicators, data elements, or other metadata. This can be done within the DHIS2 interface or via scripts if needed.

- **Editing Program Indicators**: Use the DHIS2 interface to update expressions, filters, or other configurations related to the program indicators.
- **Testing Changes**: Make sure to review the changes using the **Analytics App** and run tests to ensure that the indicators are working as expected.

---

## Testing Changes

After making the required changes in the dev environment, test the functionality of the program indicators by following these steps:

1. **Run Analytics**: Run analytics within the **Analytics App** to verify that data is being aggregated correctly.
2. **Test Reports**: Verify that the changes reflect accurately in reports or dashboards.
3. **Log Errors**: If any errors or issues arise, capture the logs and address them in the dev environment.

Once all changes are verified and functional, proceed to the next step.

---

## Promoting to Test and Production Environments

### Step 1: Export Metadata from Dev

1. Log in to your DHIS2 development instance.
2. Navigate to **Import/Export App** and select **Metadata Export**.
3. Choose the necessary objects (program indicators, data elements, etc.) for export.
4. Download the metadata export file.

### Step 2: Import Metadata to Test Environment

1. Log in to the DHIS2 test environment.
2. Navigate to the **Import/Export App**.
3. Select **Metadata Import** and upload the metadata file you exported from the dev environment.
4. Run tests to verify that the indicators and metadata are working as expected.

### Step 3: Import Metadata to Production Environment (After Testing)

Once the testing is complete and validated in the test environment:

1. Log in to the DHIS2 production environment.
2. Import the metadata using the **Import/Export App** following the same steps as before.
3. Monitor the production instance to ensure smooth deployment and no issues post-import.

---

## Contributing

If you want to contribute to this project:

- Fork the repository.
- Make your changes on a new branch.
- Open a pull request for review.

Please adhere to the coding standards and best practices mentioned in the contribution guidelines.

---
