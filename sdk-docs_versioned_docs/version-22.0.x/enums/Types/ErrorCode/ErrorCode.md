---
id: "ErrorCode"
title: "Enumeration: ErrorCode"
sidebar_label: "ErrorCode"
---

[types](../../../modules/Types/Types.md).ErrorCode

Specifies possible types of errors in the SDK

## Enumeration Members

### DataUnavailable

• **DataUnavailable** = ``"DataUnavailable"``

the data that is being fetched does not exist on-chain, or relies on non-existent data. There are
  some cases where the data did exist at some point, but has been deleted to save storage space

#### Defined in

[types/index.ts:531](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L531)

___

### EntityInUse

• **EntityInUse** = ``"EntityInUse"``

this type of error is thrown when attempting to delete/modify an entity which has other entities depending on it. For example, deleting
  a Portfolio that still holds assets, or removing a Checkpoint Schedule that is being referenced by a Corporate Action

#### Defined in

[types/index.ts:553](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L553)

___

### FatalError

• **FatalError** = ``"FatalError"``

error that should cause termination of the calling application

#### Defined in

[types/index.ts:513](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L513)

___

### General

• **General** = ``"General"``

general purpose errors that don't fit well into the other categories

#### Defined in

[types/index.ts:566](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L566)

___

### InsufficientBalance

• **InsufficientBalance** = ``"InsufficientBalance"``

one or more parties involved in the transaction do not have enough balance to perform it

#### Defined in

[types/index.ts:557](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L557)

___

### LimitExceeded

• **LimitExceeded** = ``"LimitExceeded"``

the data that is being written to the chain would result in some limit being exceeded. For example, adding a transfer
  restriction when the maximum possible amount has already been added

#### Defined in

[types/index.ts:541](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L541)

___

### MiddlewareError

• **MiddlewareError** = ``"MiddlewareError"``

errors encountered when interacting with the historic data middleware (GQL server)

#### Defined in

[types/index.ts:526](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L526)

___

### NoDataChange

• **NoDataChange** = ``"NoDataChange"``

the data that is being written to the chain is the same data that is already in place. This would result
  in a redundant/useless transaction being executed

#### Defined in

[types/index.ts:536](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L536)

___

### NotAuthorized

• **NotAuthorized** = ``"NotAuthorized"``

user does not have the required roles/permissions to perform an operation

#### Defined in

[types/index.ts:522](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L522)

___

### TransactionAborted

• **TransactionAborted** = ``"TransactionAborted"``

transaction removed from the tx pool

#### Defined in

[types/index.ts:499](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L499)

___

### TransactionRejectedByUser

• **TransactionRejectedByUser** = ``"TransactionRejectedByUser"``

user rejected the transaction in their wallet

#### Defined in

[types/index.ts:503](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L503)

___

### TransactionReverted

• **TransactionReverted** = ``"TransactionReverted"``

transaction failed due to an on-chain error. This is a business logic error,
  and it should be caught by the SDK before being sent to the chain.
  Please report it to the Polymesh team

#### Defined in

[types/index.ts:509](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L509)

___

### UnexpectedError

• **UnexpectedError** = ``"UnexpectedError"``

errors that are the result of something unforeseen.
  These should generally be reported to the Polymesh team

#### Defined in

[types/index.ts:562](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L562)

___

### UnmetPrerequisite

• **UnmetPrerequisite** = ``"UnmetPrerequisite"``

one or more base prerequisites for a transaction to be successful haven't been met. For example, reserving a ticker requires
  said ticker to not be already reserved. Attempting to reserve a ticker without that prerequisite being met would result in this
  type of error. Attempting to create an entity that already exists would also fall into this category,
  if the entity in question is supposed to be unique

#### Defined in

[types/index.ts:548](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L548)

___

### ValidationError

• **ValidationError** = ``"ValidationError"``

user input error. This means that one or more inputs passed by the user
  do not conform to expected value ranges or types

#### Defined in

[types/index.ts:518](https://github.com/PolymeshAssociation/polymesh-sdk/blob/95f248df/src/types/index.ts#L518)
