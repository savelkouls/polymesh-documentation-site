---
id: "AttestPrimaryKeyRotationParams"
title: "Interface: AttestPrimaryKeyRotationParams"
sidebar_label: "AttestPrimaryKeyRotationParams"
---

[api/procedures/types](../../../../../modules/API/Procedures/Types/Types.md).AttestPrimaryKeyRotationParams

## Properties

### expiry

• `Optional` **expiry**: `Date`

(optional) when the generated authorization should expire

#### Defined in

[api/procedures/types.ts:469](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/api/procedures/types.ts#L469)

___

### identity

• **identity**: `string` \| [`Identity`](../../../../../classes/API/Entities/Identity/Identity.md)

Identity or the DID of the Identity that is to be rotated

#### Defined in

[api/procedures/types.ts:464](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/api/procedures/types.ts#L464)

___

### targetAccount

• **targetAccount**: `string` \| [`Account`](../../../../../classes/API/Entities/Account/Account.md)

The Account that will be attested to become the primary key of the `identity`. Can be ss58 encoded address or an instance of Account

#### Defined in

[api/procedures/types.ts:459](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/api/procedures/types.ts#L459)
