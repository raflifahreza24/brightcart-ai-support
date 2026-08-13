# BrightCart AI Support Agent

## Business & System Requirements

## 1. Problem Statement

BrightCart receives a high volume of repetitive customer support
requests, including:

- Order status inquiries
- Shipping questions
- Refund policy questions
- Warranty questions
- Product recommendations
- Damaged product complaints
- Order cancellation requests

Support agents currently need to access multiple systems manually
to resolve these requests.

## 2. Business Goals

The system aims to:

- Reduce repetitive customer support workload
- Improve response time
- Provide consistent answers
- Automate low-risk support operations
- Maintain human approval for high-risk actions

## 3. User Stories

### US-01 - Order Tracking

As a customer,
I want to check my order status,
so that I know the delivery progress.

### US-02 - Knowledge Questions

As a customer,
I want to ask about refund, shipping, and warranty policies,
so that I can receive an immediate answer.

### US-03 - Product Search

As a customer,
I want product recommendations based on my requirements.

### US-04 - Complaint

As a customer,
I want to report an issue,
so that support can resolve it.

### US-05 - Human Escalation

As a support manager,
I want high-risk cases escalated,
so that sensitive decisions remain under human control.

## 4. Functional Requirements

- FR-001: System must accept customer messages.
- FR-002: System must answer questions using company knowledge.
- FR-003: System must retrieve order information.
- FR-004: System must retrieve product information.
- FR-005: System must create support tickets.
- FR-006: System must escalate sensitive requests.
- FR-007: System must record AI tool calls.
- FR-008: System must return sources for knowledge-based answers.

## 5. Non-Functional Requirements

- NFR-001: API responses should generally be under 5 seconds,
  excluding external AI latency.
- NFR-002: Customer A must not access Customer B's orders.
- NFR-003: AI must not execute arbitrary SQL.
- NFR-004: System must log important agent actions.
- NFR-005: Secrets must not be committed to Git.
- NFR-006: System must support containerized deployment.
