# Flowforge MVP Specification

## 1. Vision and Scope
- **White-label client portal & website widget**: branded interface for client onboarding and case tracking, embeddable widget for existing websites.

## 2. Core Modules

### 2.1 Intake Agent (FR/EN)
- **Functionality**:
  - Bilingual (French/English) intake assistant.
  - Generates concise case summaries.
  - Classifies matters by practice area, urgency level, and flags potential conflicts.
  - Extracts key entities (parties, dates, monetary amounts, jurisdictions).

### 2.2 Conflicts & KYC
- **Data Sources**:
  - Searches RNE/INPI registries, Pappers, public sanctions lists, and beneficial ownership data.
- **Features**:
  - Centralized party search & deduplication.
  - Automated alerts for hits or missing data.
  - Evidence capture and audit trail of checks.

### 2.3 Matter File Automation
- **Capabilities**:
  - Auto-create matters with templates based on classifications.
  - Configurable checklists and document models (letters of engagement, fee agreements).
  - Task and deadline scheduling with reminders.
  - Fee proposal generation and tracking.

### 2.4 Qualified E-signature
- Integrations with Yousign and Universign for qualified electronic signature workflows.
- Status tracking and document vault.

### 2.5 Connectors
- Native connectors with Microsoft 365, Google Workspace, Teams/Slack, SharePoint, OneDrive, and Google Drive.
- Sync documents, messages, and calendar events.

### 2.6 Administration & Compliance
- Role-based access control and granular permissions.
- Audit trail with immutable event logs.
- GDPR journal, consent management, and retention policies.
- Configurable data residency and backup settings.

## 3. User Journeys
1. **Client Onboarding**
   - Client uses white-label portal or widget.
   - Intake agent collects data, generates summary, and classifies matter.
   - Conflicts & KYC checks run automatically; flagged items assigned for review.
2. **Matter Setup**
   - Matter file created with relevant checklist and document templates.
   - Engagement letter generated and sent for qualified e-signature.
3. **Ongoing Management**
   - Tasks and deadlines tracked; teams collaborate via connected tools.
   - Admin monitors compliance via audit trails and GDPR journal.

## 4. Technical Considerations
- Modular architecture with API-first design to support portal and widget.
- Secure handling of PII and compliance data (encryption at rest/in transit).
- Logging and observability for intake agent decisions and external lookups.
- Integration framework with connector-specific adapters.

## 5. MVP Success Metrics
- Time to onboard a client reduced by 50% compared to manual process.
- 90% of matters auto-classified correctly (validated sample).
- 100% of KYC checks logged with audit trails.
- Qualified e-signature turnaround <24h on average.

## 6. Open Questions
- Licensing/usage limits for registry and sanctions data sources.
- Localisation requirements beyond FR/EN (e.g., CA, EU).
- Pricing model for white-label customization.
- Data retention durations per jurisdiction.

## 7. Next Steps
- Validate data source access and API availability.
- Prototype intake agent with bilingual prompts and evaluation rubric.
- Define checklist and template library per practice area.
- Engage legal/compliance advisors for GDPR journal structure.

