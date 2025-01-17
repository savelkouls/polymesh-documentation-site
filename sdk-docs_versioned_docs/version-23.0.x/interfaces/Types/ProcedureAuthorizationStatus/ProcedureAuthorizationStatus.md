---
id: "ProcedureAuthorizationStatus"
title: "Interface: ProcedureAuthorizationStatus"
sidebar_label: "ProcedureAuthorizationStatus"
---

[types](../../../modules/Types/Types.md).ProcedureAuthorizationStatus

## Properties

### accountFrozen

• **accountFrozen**: `boolean`

whether the Account is frozen (i.e. can't perform any transactions)

#### Defined in

[types/index.ts:1337](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/types/index.ts#L1337)

___

### agentPermissions

• **agentPermissions**: [`CheckPermissionsResult`](../CheckPermissionsResult/CheckPermissionsResult.md)<[`Identity`](../../../enums/Types/SignerType/SignerType.md#identity)\>

whether the Identity complies with all required Agent permissions

#### Defined in

[types/index.ts:1325](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/types/index.ts#L1325)

___

### noIdentity

• **noIdentity**: `boolean`

true only if the Procedure requires an Identity but the signing Account
  doesn't have one associated

#### Defined in

[types/index.ts:1342](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/types/index.ts#L1342)

___

### roles

• **roles**: [`CheckRolesResult`](../CheckRolesResult/CheckRolesResult.md)

whether the Identity complies with all required Roles

#### Defined in

[types/index.ts:1333](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/types/index.ts#L1333)

___

### signerPermissions

• **signerPermissions**: [`CheckPermissionsResult`](../CheckPermissionsResult/CheckPermissionsResult.md)<[`Account`](../../../enums/Types/SignerType/SignerType.md#account)\>

whether the Account complies with all required Signer permissions

#### Defined in

[types/index.ts:1329](https://github.com/PolymeshAssociation/polymesh-sdk/blob/720afb69c/src/types/index.ts#L1329)
