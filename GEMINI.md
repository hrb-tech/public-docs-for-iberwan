# GEMINI.md - Project Context: public-docs-for-iberwan

## Project Overview
This repository is a centralized documentation hub for applications, modules, and tasks developed by **HRB Systems** for **Iberwan/Incoway**. It is a **Non-Code Project** primarily consisting of Markdown files that serve as user and administrator manuals.

The current primary focus of this repository is the **IwQuotation** application.

## Directory Overview
- **Root**: Contains the project `README.md` and this `GEMINI.md`.
- **`iw-quotation-public-docs/`**: Contains documentation specific to the IwQuotation module, including user manuals in Portuguese (`pt_BR`).

## Key Files
- **`README.md`**: Provides a high-level summary of the repository's purpose and links to the main documentation files.
- **`iw-quotation-public-docs/iw-quotation-user-manual_pt_BR.md`**: A comprehensive user manual for the IwQuotation SPA. It covers:
    - Accessing the application via specific URLs (e.g., `App=IwQuotation&Profile=[PROFILE]`).
    - Login procedures and password management.
    - Managing "Mapas de Cotação" (Quotation Maps).
    - Detailed instructions for editing quotations, including global data, shipping (CIF/FOB), and item-specific pricing/brands.
    - Technical details regarding "Incoway" service accounts and Wildfly 20 configuration (`-DIncowayPw`).

## Usage
- **Reading Documentation**: Use these files to understand the functional and technical requirements of the Iberwan ecosystem modules.
- **Updating Docs**: When adding new modules or updating existing ones, ensure the internal links in `README.md` are maintained and follows the naming convention established in `iw-quotation-public-docs/`.

## Technical Context (IwQuotation)
- **Architecture**: Single Page Application (SPA) integrated into the `IwBrowser` system.
- **Backend**: Java-based (Wildfly 20) using `IwCare` system tables (`GLBPERSON`, `GLBUSER`, `GLBENTERPRISE`) for authentication and authorization.
- **Key Configuration**: Requires a service user named `Incoway` with its password provided via JVM Option (`IncowayPw`).
