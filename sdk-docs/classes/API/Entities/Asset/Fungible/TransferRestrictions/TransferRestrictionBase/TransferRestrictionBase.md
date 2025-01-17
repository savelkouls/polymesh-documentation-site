---
id: "TransferRestrictionBase"
title: "Class: TransferRestrictionBase<T>"
sidebar_label: "TransferRestrictionBase"
---

[api/entities/Asset/Fungible/TransferRestrictions/TransferRestrictionBase](../../../../../../../modules/API/Entities/Asset/Fungible/TransferRestrictions/TransferRestrictionBase/TransferRestrictionBase.md).TransferRestrictionBase

Base class for managing Transfer Restrictions

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`TransferRestrictionType`](../../../../../../../enums/Types/TransferRestrictionType/TransferRestrictionType.md) |

## Hierarchy

- `Namespace`<[`FungibleAsset`](../../FungibleAsset.md)\>

  ↳ **`TransferRestrictionBase`**

  ↳↳ [`ClaimCount`](../ClaimCount/ClaimCount.md)

  ↳↳ [`ClaimPercentage`](../ClaimPercentage/ClaimPercentage.md)

  ↳↳ [`Count`](../Count/Count.md)

  ↳↳ [`Percentage`](../Percentage/Percentage.md)

## Methods

### addRestriction

▸ **addRestriction**(`args`, `opts?`): `Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`BigNumber`, `BigNumber`\>\>

Add a Transfer Restriction of the corresponding type to this Asset

**`Note`**

 the result is the total amount of restrictions after the procedure has run

**`Note`**

 this method is of type [ProcedureMethod](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md), which means you can call [addRestriction.checkAuthorization](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`AddRestrictionParams`](../../../../../../../modules/API/Procedures/Types/Types.md#addrestrictionparams)<`T`\> |
| `opts?` | [`ProcedureOpts`](../../../../../../../interfaces/Types/ProcedureOpts/ProcedureOpts.md) |

#### Returns

`Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`BigNumber`, `BigNumber`\>\>

___

### disableStat

▸ **disableStat**(`args`, `opts?`): `Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`void`, `void`\>\>

Removes an Asset statistic

**`Throws`**

 if the statistic is being used or is not set

**`Note`**

 this method is of type [ProcedureMethod](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md), which means you can call [disableStat.checkAuthorization](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`RemoveAssetStatParamsBase`](../../../../../../../modules/API/Entities/Asset/Fungible/TransferRestrictions/TransferRestrictionBase/TransferRestrictionBase.md#removeassetstatparamsbase)<`T`\> |
| `opts?` | [`ProcedureOpts`](../../../../../../../interfaces/Types/ProcedureOpts/ProcedureOpts.md) |

#### Returns

`Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`void`, `void`\>\>

___

### enableStat

▸ **enableStat**(`args`, `opts?`): `Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`void`, `void`\>\>

Enables statistic of the corresponding type for this Asset, which are required for restrictions to be created

**`Note`**

 this method is of type [ProcedureMethod](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md), which means you can call [enableStat.checkAuthorization](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`SetAssetStatParams`](../../../../../../../modules/API/Procedures/Types/Types.md#setassetstatparams)<`T`\> |
| `opts?` | [`ProcedureOpts`](../../../../../../../interfaces/Types/ProcedureOpts/ProcedureOpts.md) |

#### Returns

`Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`void`, `void`\>\>

___

### get

▸ **get**(): `Promise`<[`GetTransferRestrictionReturnType`](../../../../../../../modules/API/Procedures/Types/Types.md#gettransferrestrictionreturntype)<`T`\>\>

Retrieve all active Transfer Restrictions of the corresponding type

**`Note`**

 there is a maximum number of restrictions allowed across all types.
  The `availableSlots` property of the result represents how many more restrictions can be added
  before reaching that limit

#### Returns

`Promise`<[`GetTransferRestrictionReturnType`](../../../../../../../modules/API/Procedures/Types/Types.md#gettransferrestrictionreturntype)<`T`\>\>

___

### removeRestrictions

▸ **removeRestrictions**(`opts?`): `Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`BigNumber`, `BigNumber`\>\>

Removes all Transfer Restrictions of the corresponding type from this Asset

**`Note`**

 the result is the total amount of restrictions after the procedure has run

**`Note`**

 this method is of type [NoArgsProcedureMethod](../../../../../../../interfaces/Types/NoArgsProcedureMethod/NoArgsProcedureMethod.md), which means you can call [removeRestrictions.checkAuthorization](../../../../../../../interfaces/Types/NoArgsProcedureMethod/NoArgsProcedureMethod.md#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts?` | [`ProcedureOpts`](../../../../../../../interfaces/Types/ProcedureOpts/ProcedureOpts.md) |

#### Returns

`Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`BigNumber`, `BigNumber`\>\>

___

### setRestrictions

▸ **setRestrictions**(`args`, `opts?`): `Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`BigNumber`, `BigNumber`\>\>

Sets all Transfer Restrictions of the corresponding type on this Asset

**`Note`**

 the result is the total amount of restrictions after the procedure has run

**`Note`**

 this method is of type [ProcedureMethod](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md), which means you can call [setRestrictions.checkAuthorization](../../../../../../../interfaces/Types/ProcedureMethod/ProcedureMethod.md#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`SetRestrictionsParams`](../../../../../../../modules/API/Procedures/Types/Types.md#setrestrictionsparams)<`T`\> |
| `opts?` | [`ProcedureOpts`](../../../../../../../interfaces/Types/ProcedureOpts/ProcedureOpts.md) |

#### Returns

`Promise`<[`GenericPolymeshTransaction`](../../../../../../../modules/Types/Types.md#genericpolymeshtransaction)<`BigNumber`, `BigNumber`\>\>
