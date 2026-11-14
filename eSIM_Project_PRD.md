# eSIM Subscription, Activation and Usage Management System

## Product Requirements Document (PRD)

**Project Type:** Database Systems Semester Project  
**Proposed Database:** PostgreSQL

## 1. Project Overview

The eSIM Subscription, Activation and Usage Management System is designed to manage the subscription-related operations of an eSIM service provider.

The system will maintain information about business partners, subscribers, data plans, purchases, eSIM activations, data usage and top-ups. It will help organize the subscription lifecycle, from purchasing a plan to tracking its usage and eventual expiry.

The project is based on a B2B2C business model, in which the eSIM provider works with business partners who are associated with end subscribers.

## 2. Problem Statement

Managing eSIM subscriptions involves handling different plans, network operators, subscribers, activation statuses, data allowances and subscription expiry dates.

Without a centralized system, keeping track of this information can become difficult. It may also be challenging to monitor data consumption, manage additional data purchases and identify subscriptions that are close to expiry or have already expired.

This project aims to provide a centralized database system to organize and manage these operations efficiently.

## 3. Project Objectives

The main objectives of the system are to:

- Maintain organized records of business partners and their subscribers.
- Manage available eSIM data plans and their coverage.
- Record plan purchases and subscription details.
- Track eSIM activation statuses.
- Monitor data usage and remaining data allowances.
- Manage additional data purchases (top-ups).
- Track subscription expiry, grace periods and termination.
- Generate basic reports to help monitor subscription activity.

## 4. Users and Stakeholders

The main users and stakeholders of the system include:

- **eSIM Service Provider:** Manages plans, subscriptions, usage records and overall operations.
- **Business Partners:** Organizations that work with the provider and are associated with end subscribers.
- **End Subscribers:** Customers who use the eSIM plans and consume mobile data.
- **System Administrator:** Maintains records and monitors the system's operations.

## 5. Main System Features

### 5.1 Business Partner and Subscriber Management

The system will maintain information about business partners and the subscribers associated with them. It will allow subscriber records to be organized under the relevant business partner.

### 5.2 Data Plan Management

The system will maintain available data plans, including their prices, data allowances, validity periods and country coverage.

### 5.3 Purchase and Subscription Management

The system will record plan purchases and maintain the corresponding subscription information, including start dates, expiry dates and subscription status.

A subscriber will have only one active base plan at a time.

### 5.4 eSIM Activation Tracking

The system will maintain eSIM-related information and record activation statuses so that the provider can monitor the activation state of subscriptions.

### 5.5 Data Usage Management

The system will maintain data usage records associated with subscriptions. It will help track the amount of data consumed and the remaining data allowance.

### 5.6 Top-Up Management

Subscribers will be able to purchase additional data through top-ups. The system will record these purchases and associate them with the relevant subscription.

### 5.7 Subscription Expiry and Termination

The system will monitor subscription expiry dates. Once a subscription expires, it will enter a 30-day grace period. After this period, the subscription will be marked as terminated.

### 5.8 Basic Reporting

The system will provide basic reports to help the provider monitor subscription activity. These may include active subscriptions, popular plans, data usage, top-up purchases and terminated subscriptions.

## 6. Main System Scenarios

The system is expected to handle the following situations:

1. A business partner is added to the system, and subscribers are associated with that partner.
2. A subscriber purchases an available eSIM data plan.
3. The system records the purchase and creates the corresponding subscription record.
4. The eSIM activation status is recorded and updated.
5. Data usage is recorded against the relevant subscription, allowing the remaining allowance to be monitored.
6. A subscriber purchases additional data through a top-up.
7. When a subscription reaches its expiry date, it enters the 30-day grace period.
8. After the grace period ends, the subscription is marked as terminated.
9. The provider views reports to monitor plans, subscriptions, usage and other activities.

## 7. Important Business Rules

The system will follow these basic business rules:

- Each subscriber must be associated with a valid business partner.
- Every data plan must have a defined price, data allowance and validity period.
- A data plan may provide coverage in multiple countries.
- A subscriber can have only one active base plan at a time.
- Additional data can be purchased through top-ups.
- Data usage records must be associated with a valid subscription.
- The system must keep track of consumed data and remaining allowance.
- An expired subscription will have a 30-day grace period before termination.
- A terminated subscription cannot be treated as an active subscription.

## 8. Project Scope

### 8.1 Included in the Project

The project will cover:

- Business partner and subscriber management.
- Data plan and country coverage management.
- Purchase and subscription records.
- eSIM activation status tracking.
- Data usage and remaining allowance tracking.
- Top-up purchase records.
- Subscription expiry, grace period and termination management.
- Basic operational and analytical reports.

### 8.2 Not Included in the Project

The project will not involve:

- Actual eSIM installation or provisioning on mobile devices.
- Direct control or management of telecom networks.
- Real-time measurement of mobile data traffic from devices.
- Actual payment gateway integration or payment processing.
- Development of a complete customer-facing mobile application.

The project will focus on managing and demonstrating subscription-related information through a database system. Sample or simulated records may be used where actual external operations are outside the project's scope.

## 9. Expected End Product

The expected outcome is a functional database system that provides a centralized way to manage the main operations of an eSIM service provider.

It should allow the provider to maintain partner and subscriber information, manage data plans, record purchases and subscriptions, track activation and usage, handle top-ups, and monitor subscription expiry and termination.

The system will also support basic reporting, helping the provider view and understand its subscription-related activities.