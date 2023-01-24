[api/entities/Asset/types](../../../../../Modules/API/Entities/Asset/Types.md).TransferBreakdown

Object containing every reason why a specific Asset transfer would fail

## Properties

### compliance

• **compliance**: [`Compliance`](../../../../Types/Compliance.md)

how the transfer adheres to the asset's compliance rules

#### Defined in

[api/entities/Asset/types.ts:40](https://github.com/PolymeshAssociation/polymesh-sdk/blob/15be87e8/src/api/entities/Asset/types.ts#L40)

___

### general

• **general**: [`TransferError`](../../../../../Enums/Types/TransferError.md)[]

list of general transfer errors

#### Defined in

[api/entities/Asset/types.ts:36](https://github.com/PolymeshAssociation/polymesh-sdk/blob/15be87e8/src/api/entities/Asset/types.ts#L36)

___

### restrictions

• **restrictions**: [`TransferRestrictionResult`](TransferRestrictionResult.md)[]

list of transfer restrictions and whether the transfer satisfies each one

#### Defined in

[api/entities/Asset/types.ts:44](https://github.com/PolymeshAssociation/polymesh-sdk/blob/15be87e8/src/api/entities/Asset/types.ts#L44)

___

### result

• **result**: `boolean`

true if the transfer is possible

#### Defined in

[api/entities/Asset/types.ts:48](https://github.com/PolymeshAssociation/polymesh-sdk/blob/15be87e8/src/api/entities/Asset/types.ts#L48)