---
title: Processing Service Contracts for Vehicle Service
description: 
primary_tag: 
tags: [  ]
time: 
---

<!-- loio0af8268477b6496eba13fdf9bbccabad -->

## Prerequisites

When you create a service order, you can use the order wizard to get an overview about the contracts for the customer’s vehicle.

You can select one or more service contracts in the order wizard, and copy them to the service order.

When you copy a contract to the order, the system does the following:

-   A job is created that has a service contract number and contract item.

-   The field *Split Indicator* is filled. You can define which split indicator is filled in transaction `/DBM/SPL_IND`.

-   If the *Copy Pack.* checkbox is active, the system copies all relevant packages to the order.


The service advisor can then process the order and release it to the workshop.

In the order, you can use the fast split functionality to create a split based on the [scope of work](d8a2f384558b4c71ad09233ca3c9d151.md) for the service contract item. The percentages specified in the scope of work are used for each split item. If no percentage is specified for a service contract item, the split percentage is 0. This means that the service contract does not cover this item. The billing process can be initiated after split creation.

