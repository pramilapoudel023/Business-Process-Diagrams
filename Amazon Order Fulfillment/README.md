Here's a technical README.md file for your GitHub project:

# Amazon Order Fulfillment BPMN Diagram

## Requirements
Using Microsoft Visio, create a BPMN diagram for ordering your favorite
product from Amazon Canada. To help you with the process, the order
fulfillment process overview is shared below.

## Amazon Order Fulfillment overview:
Once the customer places an order on amazon website, the order can be fulfilled (shipped) using
either of the 2 different methods – Fulfilled by Amazon (FBA) or Fulfilled by Merchant (FBM). In
FBA, the order is processed, packed, shipped, and delivered through Amazon Warehouse. In
FBM, the order is processed, packed, shipped, and delivered by the Merchant. Hence, in FBM,
Amazon only provides the digital infrastructure for receiving the order request, sending the
notifications, and collecting the online payment.
If at any point in the process, you are not sure of the step then please assume the step. This
question is to check your understanding of BPMN diagramming and not to verify the real
fulfillment process.

## Conditions for the Project
The following conditions must be met:
a. Show at least 3 different pools. For example, Customer, Amazon, Merchant, etc.
b. Show at least 4 different swim lanes (in total, not individually in a pool).
c. Show both the processes – FBA and FBM.
d. Show at least 20 different flow objects – Activity/Task, Gateway, and Event are
considered as flow objects.
e. Show at least 3 different types of Gateways and at least 3 different types of Activity/Task.

## Project Description
A Business Process Model and Notation (BPMN) 2.0 diagram modeling Amazon Canada's order fulfillment process, covering both Fulfilled-by-Amazon (FBA) and Fulfilled-by-Merchant (FBM) workflows. Created using Microsoft Visio.

## Key Features
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
