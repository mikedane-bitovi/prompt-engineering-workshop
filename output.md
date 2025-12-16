# Todo List Requirements Document

## Assumptions
- The todo list will be used by pilots within the aviation company.
- Each pilot has a unique user account.
- The system will be accessed via secure company devices.
- The todo list is not flight-critical but must not interfere with flight operations.
- The backend will be implemented in C++ by a senior engineer.
- The system will integrate with existing authentication infrastructure.

## Overview
This document defines the requirements for a secure todo list application for pilots. The focus is on ensuring data confidentiality, integrity, and availability, with strong emphasis on security and auditability.

## Functional Requirements

- **TODO-1:** Access to the todo list must be restricted to authenticated users only.
- **TODO-2:** Pilots can only view and modify their own todo lists.
- **TODO-3:** All changes to todo items must be logged with user ID and timestamp.
- **TODO-4:** Only authenticated users can modify their own todo items.

## Non-Functional Requirements

- **TODO-5:** All data at rest and in transit must be encrypted using industry-standard algorithms.
- **TODO-6:** The system must validate all user input to prevent injection attacks.
- **TODO-7:** The todo list service must be available 99.9% of the time, excluding scheduled maintenance.

## Open Questions

- What is the maximum number of todo items per user?
- Should deleted todo items be recoverable (soft delete) or permanently removed?
- What is the required retention period for audit logs?
- Are there any regulatory requirements specific to aviation data storage?
# Todo List Requirements Document

## Assumptions

## Overview
## Assumptions
- The todo list will be used by pilots and aviation staff with varying levels of technical expertise.
- The application will be deployed in a secure aviation environment with network access controls.
- User authentication and authorization are managed by an existing company-wide identity provider.
- The todo list may contain sensitive operational or personal information.
- The backend will be implemented in C++ by a senior engineer.
- The system will be accessed via secure company devices.

## Overview
This document outlines the requirements for a secure, reliable todo list application for pilots. The focus is on ensuring data confidentiality, integrity, and availability, while supporting essential task management features.

## Functional Requirements
- **TODO-1:** The system SHALL require user authentication before granting access to any todo list data.
- **TODO-2:** The system SHALL allow authenticated users to create, read, update, and delete their own todo items.
- **TODO-3:** The system SHALL prevent users from accessing or modifying todo items belonging to other users.
- **TODO-4:** The system SHALL log all access and modification events to todo items, including user ID, timestamp, and action performed.
- **TODO-5:** The system SHALL support marking todo items as completed or pending.

## Non-Functional Requirements
- **TODO-6:** All data in transit SHALL be encrypted using TLS 1.2 or higher.
- **TODO-7:** All todo list data at rest SHALL be encrypted using AES-256 or equivalent.
- **TODO-8:** The system SHALL reject any input containing SQL injection, command injection, or XSS attack patterns.
- **TODO-9:** The system SHALL respond to all requests within 2 seconds under normal operating conditions (≤100 concurrent users).
- **TODO-10:** The system SHALL be available 99.9% of the time, excluding scheduled maintenance.

## Open Questions
- What is the maximum expected number of concurrent users?
- Should todo items support attachments (e.g., documents, images)?
- Are there regulatory requirements for data retention or audit logging?
- What is the required data backup and disaster recovery policy?

## Functional Requirements
- **TODO-1:** The system SHALL require user authentication before granting access to any todo list data.
- **TODO-2:** The system SHALL allow authenticated users to create, read, update, and delete their own todo items only.
- **TODO-3:** The system SHALL log all access and modification events to todo items, including user ID, timestamp, and action performed.
- **TODO-4:** The system SHALL enforce input validation to prevent injection attacks and reject malformed or malicious data.
- **TODO-5:** The system SHALL encrypt all todo item data at rest and in transit using industry-standard encryption protocols.

## Non-Functional Requirements
- **TODO-6:** The system SHALL respond to all authorized requests within 2 seconds under normal operating conditions.
- **TODO-7:** The system SHALL be resilient to at least 3 consecutive failed login attempts by locking the account for 15 minutes.
- **TODO-8:** The system SHALL retain audit logs for a minimum of 12 months and protect them from unauthorized modification or deletion.
- **TODO-9:** The system SHALL comply with relevant aviation cybersecurity regulations and company security policies.

## Open Questions
- What is the maximum number of todo items a user may store?
- Are there any specific regulatory standards (e.g., DO-326A) that must be referenced for compliance?
- Should the system support shared todo lists between multiple users or teams?
- What is the required disaster recovery time objective (RTO) for this application?
