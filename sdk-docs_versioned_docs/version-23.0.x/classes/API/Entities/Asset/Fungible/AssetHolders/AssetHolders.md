---
id: "AssetHolders"
title: "Class: AssetHolders"
sidebar_label: "AssetHolders"
---

[api/entities/Asset/Fungible/AssetHolders](../../../../../../modules/API/Entities/Asset/Fungible/AssetHolders/AssetHolders.md).AssetHolders

Handles all Asset Holders related functionality

## Hierarchy

- `Namespace`<[`FungibleAsset`](../FungibleAsset.md)\>

  ↳ **`AssetHolders`**

## Methods

### get

▸ **get**(`paginationOpts?`): `Promise`<[`ResultSet`](../../../../../../interfaces/Types/ResultSet/ResultSet.md)<[`IdentityBalance`](../../../../../../interfaces/API/Entities/Asset/Types/IdentityBalance/IdentityBalance.md)\>\>

Retrieve all the Asset Holders with their respective balance

**`Note`**

 supports pagination

#### Parameters

| Name | Type |
| :------ | :------ |
| `paginationOpts?` | [`PaginationOptions`](../../../../../../interfaces/Types/PaginationOptions/PaginationOptions.md) |

#### Returns

`Promise`<[`ResultSet`](../../../../../../interfaces/Types/ResultSet/ResultSet.md)<[`IdentityBalance`](../../../../../../interfaces/API/Entities/Asset/Types/IdentityBalance/IdentityBalance.md)\>\>
