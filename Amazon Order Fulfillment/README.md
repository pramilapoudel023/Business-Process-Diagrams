Here's a technical README.md file for your GitHub project:

# Amazon Order Fulfillment BPMN Diagram

## Project Description
A Business Process Model and Notation (BPMN) 2.0 diagram modeling Amazon Canada's order fulfillment process, covering both Fulfilled-by-Amazon (FBA) and Fulfilled-by-Merchant (FBM) workflows. Created using Microsoft Visio.

## Key Features
- **Compliant with assignment requirements**:
  - 3 Pools: Customer, Amazon, Merchant
  - 4 Swimlanes across pools
  - Dual process flows (FBA & FBM)
  - 24 Flow Objects (12 Tasks, 6 Gateways, 6 Events)
  - Multiple gateway types (Exclusive, Parallel, Event-Based)
  - Task types (User, Service, Send/Receive)

## Diagram Overview
Process Diagram Preview

**Core Components**:
1. **Order Initiation**:
   - Customer places order
   - Payment processing
   - Order confirmation

2. **Fulfillment Paths**:
   ```plaintext
   FBA Path:
   Customer → Amazon Warehouse (Pick/Pack) → Amazon Shipping → Delivery

   FBM Path: 
   Customer → Merchant System (Pick/Pack) → Merchant Shipping → Delivery
   ```

3. **Key Decision Points**:
   | Gateway Type | Location | Decision Criteria |
   |--------------|----------|-------------------|
   | Exclusive    | Stock Check | Item availability[1] |
   | Parallel     | Payment Processing | Multiple payment methods |
   | Event-Based  | Shipping Update | Tracking notifications |

## BPMN Elements Breakdown
**Flow Objects** (24 total):
- **Tasks**:
  - User Task: Product selection
  - Service Task: Payment processing
  - Send Task: Shipping notifications

- **Gateways**:
  - Exclusive (XOR)
  - Parallel (AND)
  - Event-Based

- **Events**:
  - Start: Order placement
  - Intermediate: Shipping updates
  - End: Delivery confirmation

## Setup & Usage
1. **Requirements**:
   - Microsoft Visio 2019+
   - BPMN 2.0 stencil

2. **Open in Visio**:
   - Launch `AmazonFulfillmentProcess.vsdx`
   - Enable BPMN 2.0 validation

## Assumptions Made
- Simplified inventory check process
- Combined payment processing steps
- Generalized shipping carrier selection
